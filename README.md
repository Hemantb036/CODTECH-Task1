# CODTECH-Task1
Password Strength Meter For angular 6
To display the strength of the password with a visual feedback.

Password Strength Meter use zxcvbn to estimate the strength of the password and also provide a visual feedback with suggestions and warning messages.

This lib was developed based on the following tutorial.

How then is password strength measured? Dropbox developed an algorithm for a realistic password strength estimator inspired by password crackers. This algorithm is packaged in a Javascript library called zxcvbn. In addition, the package contains a dictionary of commonly used English words, names and passwords.

Demo
See Demo Here

  <password-strength-meter [password]="password"></password-strength-meter>
Get Started
Step 1: Since this lib was depending upon the zxcvbn lib, install it first

npm install zxcvbn@4.4.2 --save
Step 2: Install password-strength-meter

npm install angular-password-strength-meter --save
Step 3: Import Password Strength Meter Module into your app module

....
import { PasswordStrengthMeterModule } from 'angular-password-strength-meter';

....

@NgModule({
    ...
    imports: [
        ....
        PasswordStrengthMeterModule
    ],
    ....
})
export class AppModule { }
Step 4: use the password-strength-meter component in your app.component.ts

  <password-strength-meter [password]="password"></password-strength-meter>
API
