# Coach Catalyst - Sign Up Test Cases

## Module: User Registration & Onboarding
**Priority**: P0 - Critical  
**Testing Scope**: Web Platform, Mobile Apps (Android + iOS)

---

## Test Case 1: Valid User Sign Up

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-001 |
| **Test Case Title** | Valid User Sign Up |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Enter valid first name: "Test"<br>3. Enter valid last name: "User"<br>4. Enter valid email: "testuser@example.com"<br>5. Enter valid password: "TestPass123!"<br>6. Click "Get Started" button |
| **Expected Result** | User is redirected to OTP verification page |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 2: Empty First Name Validation

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-002 |
| **Test Case Title** | Empty First Name Validation |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Leave first name field empty<br>3. Enter valid last name: "User"<br>4. Enter valid email: "test@example.com"<br>5. Enter valid password: "TestPass123!"<br>6. Click "Get Started" button |
| **Expected Result** | Validation error message displays for first name field |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 3: Empty Last Name Validation

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-003 |
| **Test Case Title** | Empty Last Name Validation |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Enter valid first name: "Test"<br>3. Leave last name field empty<br>4. Enter valid email: "test@example.com"<br>5. Enter valid password: "TestPass123!"<br>6. Click "Get Started" button |
| **Expected Result** | Validation error message displays for last name field |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 4: Empty Email Validation

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-004 |
| **Test Case Title** | Empty Email Validation |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Enter valid first name: "Test"<br>3. Enter valid last name: "User"<br>4. Leave email field empty<br>5. Enter valid password: "TestPass123!"<br>6. Click "Get Started" button |
| **Expected Result** | Validation error message displays for email field |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 5: Empty Password Validation

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-005 |
| **Test Case Title** | Empty Password Validation |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Enter valid first name: "Test"<br>3. Enter valid last name: "User"<br>4. Enter valid email: "test@example.com"<br>5. Leave password field empty<br>6. Click "Get Started" button |
| **Expected Result** | Validation error message displays for password field |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 6: Invalid Email Format Validation

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-006 |
| **Test Case Title** | Invalid Email Format Validation |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Enter valid first name: "Test"<br>3. Enter valid last name: "User"<br>4. Enter invalid email: "invalid-email"<br>5. Enter valid password: "TestPass123!"<br>6. Click "Get Started" button |
| **Expected Result** | Validation error message displays for invalid email format |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 7: Duplicate Email Validation

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-007 |
| **Test Case Title** | Duplicate Email Validation |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page, existing account with email exists |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Enter valid first name: "Test"<br>3. Enter valid last name: "User"<br>4. Enter existing email: "chinonsochibuzor5+1@gmail.com"<br>5. Enter valid password: "TestPass123!"<br>6. Click "Get Started" button |
| **Expected Result** | Error message displays indicating email already exists |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 8: Weak Password Validation

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-008 |
| **Test Case Title** | Weak Password Validation |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Enter valid first name: "Test"<br>3. Enter valid last name: "User"<br>4. Enter valid email: "test@example.com"<br>5. Enter weak password: "123"<br>6. Click "Get Started" button |
| **Expected Result** | Validation error message displays for weak password |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 9: Pre-filled Data Handling

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-009 |
| **Test Case Title** | Pre-filled Data Handling |
| **Module** | Sign Up |
| **Priority** | P1 |
| **Test Type** | UI/UX |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Verify if fields are pre-filled with "John", "Doe", "john@example.com"<br>3. Test editing pre-filled values<br>4. Test clearing pre-filled values<br>5. Submit form with pre-filled data |
| **Expected Result** | Pre-filled data can be edited or cleared, form submission works with pre-filled data |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 10: Terms and Privacy Policy Links

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-010 |
| **Test Case Title** | Terms and Privacy Policy Links |
| **Module** | Sign Up |
| **Priority** | P1 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Click "terms of service" link<br>3. Verify link opens in new tab/window<br>4. Close and click "privacy policy" link<br>5. Verify link opens in new tab/window |
| **Expected Result** | Both links open in new tabs with proper content |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 11: OTP Verification Process

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-011 |
| **Test Case Title** | OTP Verification Process |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User has completed sign-up form and is on OTP page |
| **Test Steps** | 1. Complete sign-up form with valid data<br>2. Click "Get Started" button<br>3. Verify redirect to OTP verification page<br>4. Check email for OTP code<br>5. Enter 6-digit OTP code<br>6. Click "Verify" button |
| **Expected Result** | OTP verification succeeds and user is redirected to next step |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 12: Invalid OTP Entry

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-012 |
| **Test Case Title** | Invalid OTP Entry |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on OTP verification page |
| **Test Steps** | 1. Enter incorrect 6-digit OTP code<br>2. Click "Verify" button<br>3. Verify error message displays<br>4. Test with partial OTP (less than 6 digits)<br>5. Test with non-numeric characters |
| **Expected Result** | Error messages display for invalid OTP entries |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 13: Resend OTP Functionality

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-013 |
| **Test Case Title** | Resend OTP Functionality |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on OTP verification page |
| **Test Steps** | 1. Wait for OTP or click "Resend OTP" link<br>2. Verify new OTP is sent<br>3. Check email for new OTP<br>4. Enter new OTP code<br>5. Click "Verify" button |
| **Expected Result** | Resend OTP functionality works and new OTP is valid |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 14: OTP Expiration Handling

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-014 |
| **Test Case Title** | OTP Expiration Handling |
| **Module** | Sign Up |
| **Priority** | P1 |
| **Test Type** | Functional |
| **Preconditions** | User is on OTP verification page |
| **Test Steps** | 1. Wait for OTP to expire (if applicable)<br>2. Try to verify with expired OTP<br>3. Verify appropriate error message<br>4. Test resend functionality after expiration |
| **Expected Result** | Expired OTP is rejected with appropriate error message |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 15: Onboarding Flow - Personal Tab

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-015 |
| **Test Case Title** | Onboarding Flow - Personal Tab |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User has completed OTP verification |
| **Test Steps** | 1. Complete OTP verification<br>2. Verify redirect to onboarding Personal tab<br>3. Test Coach Type dropdown selection<br>4. Test Teammates selection<br>5. Test Clients selection<br>6. Test Location selection<br>7. Click "NEXT" button |
| **Expected Result** | All dropdown selections work and user can proceed to next tab |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 16: Onboarding Flow - Business Tab

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-016 |
| **Test Case Title** | Onboarding Flow - Business Tab |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on Business tab of onboarding |
| **Test Steps** | 1. Navigate to Business tab<br>2. Enter organization name<br>3. Select brand color<br>4. Enter problem statement (optional)<br>5. Click "NEXT" button |
| **Expected Result** | Business information is saved and user can proceed to next tab |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 17: Onboarding Flow - Get the App Tab

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-017 |
| **Test Case Title** | Onboarding Flow - Get the App Tab |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Functional |
| **Preconditions** | User is on Get the App tab of onboarding |
| **Test Steps** | 1. Navigate to Get the App tab<br>2. Select country code<br>3. Enter phone number<br>4. Click "Let's Go!" button<br>5. Verify redirect to dashboard |
| **Expected Result** | Phone number is saved and user is redirected to dashboard |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 18: Input Length Validation

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-018 |
| **Test Case Title** | Input Length Validation |
| **Module** | Sign Up |
| **Priority** | P1 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Test very long inputs:<br>   - First name: 100+ characters<br>   - Last name: 100+ characters<br>   - Email: 100+ characters<br>   - Password: 100+ characters<br>3. Click "Get Started" button |
| **Expected Result** | Long inputs are handled appropriately without breaking UI |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 19: Special Characters in Names

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-019 |
| **Test Case Title** | Special Characters in Names |
| **Module** | Sign Up |
| **Priority** | P1 |
| **Test Type** | Functional |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Enter first name with special characters: "Test@#$%"<br>3. Enter last name with special characters: "User!@#$%"<br>4. Enter valid email: "test@example.com"<br>5. Enter valid password: "TestPass123!"<br>6. Click "Get Started" button |
| **Expected Result** | Special characters in names are handled appropriately |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 20: Cross-Browser Sign Up

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-020 |
| **Test Case Title** | Cross-Browser Sign Up |
| **Module** | Sign Up |
| **Priority** | P1 |
| **Test Type** | Compatibility |
| **Preconditions** | User has valid test data |
| **Test Steps** | 1. Test sign-up in Chrome<br>2. Test sign-up in Firefox<br>3. Test sign-up in Safari<br>4. Test sign-up in Edge<br>5. Verify consistent behavior across browsers |
| **Expected Result** | Sign-up process works consistently across all browsers |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 21: Mobile Sign Up

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-021 |
| **Test Case Title** | Mobile Sign Up |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Mobile |
| **Preconditions** | User is on mobile device |
| **Test Steps** | 1. Open mobile app or mobile browser<br>2. Navigate to sign-up page<br>3. Complete sign-up form<br>4. Complete OTP verification<br>5. Complete onboarding flow |
| **Expected Result** | Sign-up process works on mobile device |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 22: Security Testing - XSS Prevention

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-022 |
| **Test Case Title** | Security Testing - XSS Prevention |
| **Module** | Sign Up |
| **Priority** | P0 |
| **Test Type** | Security |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Enter XSS attempt in first name: "<script>alert('XSS')</script>"<br>3. Enter XSS attempt in last name: "<img src=x onerror=alert('XSS')>"<br>4. Enter valid email: "test@example.com"<br>5. Enter valid password: "TestPass123!"<br>6. Click "Get Started" button |
| **Expected Result** | XSS attempts are blocked and handled securely |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 23: Accessibility Testing

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-023 |
| **Test Case Title** | Accessibility Testing |
| **Module** | Sign Up |
| **Priority** | P2 |
| **Test Type** | Accessibility |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Test keyboard navigation (Tab, Enter)<br>3. Test with screen reader<br>4. Verify ARIA labels<br>5. Test color contrast<br>6. Test form validation accessibility |
| **Expected Result** | Sign-up page is accessible and navigable with assistive technologies |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 24: Performance Testing

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-024 |
| **Test Case Title** | Performance Testing |
| **Module** | Sign Up |
| **Priority** | P2 |
| **Test Type** | Performance |
| **Preconditions** | User has valid test data |
| **Test Steps** | 1. Navigate to sign-up page<br>2. Measure page load time<br>3. Complete sign-up form and measure submission time<br>4. Test OTP verification performance<br>5. Test onboarding flow performance |
| **Expected Result** | Sign-up process is responsive and performs well |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Test Case 25: Error Message Consistency

| Field | Value |
|-------|-------|
| **Test ID** | TC-SIGNUP-025 |
| **Test Case Title** | Error Message Consistency |
| **Module** | Sign Up |
| **Priority** | P1 |
| **Test Type** | UI/UX |
| **Preconditions** | User is on sign-up page |
| **Test Steps** | 1. Test various error scenarios:<br>   - Empty fields<br>   - Invalid email format<br>   - Weak password<br>   - Duplicate email<br>2. Verify error message consistency and clarity |
| **Expected Result** | Error messages are consistent, clear, and helpful |
| **Actual Result** | [To be filled during execution] |
| **Status** | [To be filled during execution] |
| **Notes** | [To be filled during execution] |
| **Screenshots** | [To be filled during execution] |
| **Browser/Device** | [To be filled during execution] |

---

## Summary

**Total Test Cases**: 25  
**Critical (P0)**: 8  
**High Priority (P1)**: 12  
**Medium Priority (P2)**: 5  

**Key Areas Covered**:
- Form validation and input handling
- OTP verification process
- Onboarding flow completion
- Security vulnerability testing
- Cross-platform compatibility
- Accessibility compliance
- Performance validation
- Error message consistency

**Execution Notes**:
- Execute P0 tests first to ensure critical functionality
- Pay special attention to input validation and security
- Test complete sign-up to onboarding flow
- Document all validation errors and security issues
- Verify OTP functionality works reliably
- Test across multiple browsers and devices