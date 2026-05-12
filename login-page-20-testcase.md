# Login Page Manual Test Cases

## TC001 - Valid Login
- Type a valid email
- Type the correct password
- Click the login button
- Expected Result: User logs in successfully

## TC002 - Invalid Password
- Type a valid email
- Type a wrong password
- Click login
- Expected Result: An error message is shown

## TC003 - Empty Email Field
- Leave the email field blank
- Type a password
- Click login
- Expected Result: Email validation message is shown

## TC004 - Empty Password
- Type an email
- Leave the password field blank
- Click login
- Expected Result: Password required message is shown

## TC005 - Invalid Email Format
- Type an invalid email (missing @ or domain)
- Type a password
- Click login
- Expected Result: Invalid email format message is shown

## TC006 - Both Fields Empty
- Leave email and password blank
- Click login
- Expected Result: Both validation messages are shown

## TC007 - Email With Spaces
- Type an email with spaces before or after it
- Type a valid password
- Click login
- Expected Result: Spaces are trimmed and login works

## TC008 - Password With Spaces
- Type a valid email
- Type a password with spaces before or after it
- Click login
- Expected Result: System handles it per spec (trim or treat as-is)

## TC009 - Email Case Insensitivity
- Type a valid email using different letter case
- Type a valid password
- Click login
- Expected Result: Login succeeds if email is case-insensitive

## TC010 - Password Case Sensitivity
- Type a valid email
- Type the password with different letter case
- Click login
- Expected Result: Login fails and an error message appears

## TC011 - Unregistered Email
- Type an email that is not registered
- Type any password
- Click login
- Expected Result: Account not found or invalid credentials message

## TC012 - Locked Account
- Type the email of a locked account
- Type the correct password
- Click login
- Expected Result: Account locked message is shown

## TC013 - Disabled Account
- Type the email of a disabled account
- Type the correct password
- Click login
- Expected Result: Account disabled message is shown

## TC014 - Forgot Password Link
- Click the Forgot Password link
- Expected Result: User is taken to the password reset page

## TC015 - Remember Me Checked
- Check Remember Me
- Enter valid credentials
- Click login
- Expected Result: User stays logged in after closing and reopening the browser (per requirement)

## TC016 - Remember Me Unchecked
- Keep Remember Me unchecked
- Enter valid credentials
- Click login
- Expected Result: Session ends after the browser is closed (per requirement)

## TC017 - Password Masking
- Type a password
- Expected Result: Password characters are hidden/masked

## TC018 - Show/Hide Password Toggle
- Click the show/hide password icon
- Expected Result: Password visibility toggles correctly

## TC019 - Login Button Disabled Until Valid Input
- Check the login button with empty or invalid fields
- Enter valid email and password
- Expected Result: Button enables only when input is valid (if implemented)

## TC020 - Multiple Failed Attempts
- Type a valid email
- Enter the wrong password repeatedly up to the limit
- Click login each time
- Expected Result: Rate limit, captcha, or lockout message appears after the threshold
