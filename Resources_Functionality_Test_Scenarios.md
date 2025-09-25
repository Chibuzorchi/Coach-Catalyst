# Coach Catalyst - Resources Functionality Test Scenarios

## Table of Contents
1. [Resources Page Navigation](#resources-page-navigation)
2. [Folder Creation Testing](#folder-creation-testing)
3. [Cover Image Management](#cover-image-management)
4. [File Upload Testing](#file-upload-testing)
5. [Video Management Testing](#video-management-testing)
6. [Link Management Testing](#link-management-testing)
7. [Resource Management Testing](#resource-management-testing)
8. [Client Sharing Testing](#client-sharing-testing)
9. [Folder Options Testing](#folder-options-testing)
10. [Cross-Browser & Device Testing](#cross-browser--device-testing)
11. [Performance & Security Testing](#performance--security-testing)
12. [Edge Cases & Error Handling](#edge-cases--error-handling)

---

## Resources Page Navigation

### 1. Resources Tab Access
**Test Case**: Verify Resources tab navigation
**Steps**:
1. Login to the platform
2. Click on "Resources" tab in the left sidebar
3. Verify URL changes to `app.coachcatalyst.com/organization_resources`
4. Verify Resources page loads correctly

**Expected Result**: Resources page loads with empty state message
**Priority**: High

### 2. Empty State Display
**Test Case**: Verify empty state when no folders exist
**Steps**:
1. Navigate to Resources page
2. Verify empty state message displays
3. Verify "Add Folder" button is visible
4. Verify folder icon with plus sign is displayed

**Expected Result**: 
- "No folders have been created yet" message
- "Click the 'Add Folder' button to create your first folder" instruction
- "Add Folder" button is prominent and clickable

**Priority**: High

### 3. Trial Banner Display
**Test Case**: Verify trial banner is displayed
**Steps**:
1. Navigate to Resources page
2. Verify green trial banner at top
3. Verify trial days remaining count
4. Click "Click here to upgrade now" link

**Expected Result**: 
- Banner shows "Your trial has 14 day(s) remaining"
- Upgrade link is clickable and functional

**Priority**: Medium

---

## Folder Creation Testing

### 4. Create New Folder Modal
**Test Case**: Verify "Add Folder" button opens modal
**Steps**:
1. Click "Add Folder" button
2. Verify modal opens with title "Create New Folder"
3. Verify folder name input field is present
4. Verify "Cancel" and "Create Folder" buttons are present

**Expected Result**: 
- Modal opens centered on screen
- Input field has placeholder "Enter a unique name for your folder"
- Buttons are properly styled and clickable

**Priority**: High

### 5. Folder Name Validation
**Test Case**: Test folder name input validation
**Steps**:
1. Open "Create New Folder" modal
2. Leave folder name field empty
3. Click "Create Folder" button
4. Test with various invalid inputs:
   - Special characters only
   - Very long names (100+ characters)
   - Names with only spaces
   - Names with HTML tags

**Expected Result**: 
- Empty field shows validation error
- Invalid inputs are rejected with appropriate error messages
- Modal remains open until valid input provided

**Priority**: High

### 6. Valid Folder Creation
**Test Case**: Create folder with valid name
**Steps**:
1. Open "Create New Folder" modal
2. Enter valid folder name (e.g., "Test Folder")
3. Click "Create Folder" button
4. Verify folder is created and modal closes
5. Verify folder appears in resources list

**Expected Result**: 
- Folder is created successfully
- Modal closes automatically
- New folder appears with "0 files" indicator
- Folder name is displayed correctly

**Priority**: High

### 7. Duplicate Folder Name Handling
**Test Case**: Test duplicate folder name creation
**Steps**:
1. Create a folder with name "Test Folder"
2. Try to create another folder with same name
3. Verify system response

**Expected Result**: 
- System prevents duplicate folder names
- Appropriate error message displayed
- Modal remains open for correction

**Priority**: High

### 8. Cancel Folder Creation
**Test Case**: Test cancel button functionality
**Steps**:
1. Open "Create New Folder" modal
2. Enter folder name
3. Click "Cancel" button
4. Verify modal closes without creating folder

**Expected Result**: 
- Modal closes without saving
- No folder is created
- User returns to resources page

**Priority**: Medium

---

## Cover Image Management

### 9. Cover Image Card Display
**Test Case**: Verify cover image card in folder
**Steps**:
1. Create a new folder
2. Open the folder
3. Verify "Add cover image" card is displayed
4. Verify card shows "PNG or JPG up to 25MB" description
5. Verify "From computer" and "From Unsplash" buttons

**Expected Result**: 
- Card is prominently displayed (darker background)
- Both buttons are clickable
- Description text is clear and informative

**Priority**: High

### 10. Upload Cover Image from Computer
**Test Case**: Test file upload from computer
**Steps**:
1. Click "From computer" button in cover image card
2. Select valid image file (PNG/JPG)
3. Verify file upload process
4. Test with invalid file types (TXT, DOC, etc.)
5. Test with oversized files (>25MB)

**Expected Result**: 
- File picker opens for valid file types
- Valid images upload successfully
- Invalid files are rejected with error message
- Oversized files show appropriate error

**Priority**: High

### 11. Unsplash Integration
**Test Case**: Test Unsplash image selection
**Steps**:
1. Click "From Unsplash" button
2. Verify Unsplash modal opens
3. Verify search functionality works
4. Test search with various keywords
5. Select an image and click "Select Image"

**Expected Result**: 
- Modal opens with Unsplash interface
- Search returns relevant results
- Image selection works correctly
- Selected image becomes cover image

**Priority**: High

### 12. Unsplash Search Functionality
**Test Case**: Test Unsplash search features
**Steps**:
1. Open Unsplash modal
2. Test search with predefined tags:
   - health, plant, nature, abstract
   - animal, wallpaper, business, art
   - colorful, food, texture, portrait
   - space, technology, architecture, exercise, patterns
3. Test custom search terms
4. Test search with empty query
5. Test search with special characters

**Expected Result**: 
- All predefined tags work correctly
- Custom search returns relevant results
- Empty search shows appropriate message
- Special characters are handled properly

**Priority**: Medium

### 13. Cover Image Edit Functionality
**Test Case**: Test cover image editing options
**Steps**:
1. Add a cover image to folder
2. Hover over the cover image
3. Verify "Edit Image" option appears
4. Test "From computer" and "From Unsplash" options
5. Test image replacement

**Expected Result**: 
- Hover shows edit options
- Both replacement methods work
- New image replaces old one
- Changes are saved correctly

**Priority**: Medium

---

## File Upload Testing

### 14. File Upload Card Display
**Test Case**: Verify file upload card
**Steps**:
1. Open a folder
2. Verify "Upload or drop files" card is displayed
3. Verify supported file types are listed
4. Verify "From computer" button is present

**Expected Result**: 
- Card shows "PNG, JPG, GIF, MPEG, or PDF up to 25MB"
- Upload button is clickable
- Drag and drop area is indicated

**Priority**: High

### 15. File Upload from Computer
**Test Case**: Test file upload functionality
**Steps**:
1. Click "From computer" button
2. Upload various file types:
   - PNG image
   - JPG image
   - GIF image
   - MPEG video
   - PDF document
3. Test with unsupported file types
4. Test with oversized files

**Expected Result**: 
- Supported files upload successfully
- Unsupported files are rejected
- Oversized files show error message
- Files appear in folder after upload

**Priority**: High

### 16. Drag and Drop Upload
**Test Case**: Test drag and drop functionality
**Steps**:
1. Drag valid file over upload area
2. Drop file in upload area
3. Verify file uploads automatically
4. Test with multiple files
5. Test with invalid file types

**Expected Result**: 
- Drag and drop works for valid files
- Multiple files upload correctly
- Invalid files are rejected
- Visual feedback during drag operation

**Priority**: Medium

### 17. File Size Validation
**Test Case**: Test file size limits
**Steps**:
1. Try to upload files of various sizes:
   - 1MB file
   - 10MB file
   - 25MB file (limit)
   - 30MB file (over limit)
2. Verify size validation messages

**Expected Result**: 
- Files under 25MB upload successfully
- Files over 25MB are rejected
- Clear error messages for oversized files

**Priority**: High

---

## Video Management Testing

### 18. Add Video Card Display
**Test Case**: Verify add video card
**Steps**:
1. Open a folder
2. Verify "Add Video" card is displayed
3. Verify description shows supported platforms
4. Verify "Add Video URL" button is present

**Expected Result**: 
- Card shows "YouTube, Vimeo or Wistia Video URL"
- Button is clickable
- Description is clear and informative

**Priority**: High

### 19. Add Video Modal
**Test Case**: Test add video modal functionality
**Steps**:
1. Click "Add Video URL" button
2. Verify modal opens with title "Add Hosted Video"
3. Verify form fields are present:
   - Video Title input
   - Video URL input
4. Verify buttons are present:
   - Cancel
   - Add Video

**Expected Result**: 
- Modal opens correctly
- All form fields are present and functional
- Buttons are properly styled

**Priority**: High

### 20. Video URL Validation
**Test Case**: Test video URL validation
**Steps**:
1. Open add video modal
2. Test with various URL formats:
   - Valid YouTube URL
   - Valid Vimeo URL
   - Valid Wistia URL
   - Invalid URL formats
   - Non-video URLs
3. Test with empty fields
4. Test with very long URLs

**Expected Result**: 
- Valid video URLs are accepted
- Invalid URLs are rejected with error messages
- Empty fields show validation errors
- Long URLs are handled appropriately

**Priority**: High

### 21. Video Title Validation
**Test Case**: Test video title input
**Steps**:
1. Open add video modal
2. Test with various title inputs:
   - Valid title
   - Empty title
   - Very long title
   - Title with special characters
3. Verify title is required

**Expected Result**: 
- Valid titles are accepted
- Empty title shows validation error
- Long titles are handled appropriately
- Special characters are allowed

**Priority**: Medium

### 22. Video Addition Success
**Test Case**: Test successful video addition
**Steps**:
1. Open add video modal
2. Enter valid video title
3. Enter valid video URL
4. Click "Add Video" button
5. Verify video is added to folder

**Expected Result**: 
- Video is added successfully
- Modal closes automatically
- Video appears in folder with correct title
- Video thumbnail is displayed

**Priority**: High

---

## Link Management Testing

### 23. Add Link Card Display
**Test Case**: Verify add link card
**Steps**:
1. Open a folder
2. Verify "Add Link" card is displayed
3. Verify description shows "URL of an external link"
4. Verify "Add Link" button is present

**Expected Result**: 
- Card is clearly displayed
- Button is clickable
- Description is informative

**Priority**: High

### 24. Add Link Modal
**Test Case**: Test add link modal functionality
**Steps**:
1. Click "Add Link" button
2. Verify modal opens with title "Add External Link"
3. Verify form fields are present:
   - Display Name input
   - URL input
4. Verify buttons are present:
   - Cancel
   - Add Link

**Expected Result**: 
- Modal opens correctly
- All form fields are present
- Buttons are properly styled

**Priority**: High

### 25. Link URL Validation
**Test Case**: Test link URL validation
**Steps**:
1. Open add link modal
2. Test with various URL formats:
   - Valid HTTP URL
   - Valid HTTPS URL
   - Invalid URL formats
   - URLs without protocol
   - Very long URLs
3. Test with empty URL field

**Expected Result**: 
- Valid URLs are accepted
- Invalid URLs are rejected with error messages
- Empty URL shows validation error
- Long URLs are handled appropriately

**Priority**: High

### 26. Display Name Validation
**Test Case**: Test display name input
**Steps**:
1. Open add link modal
2. Test with various display names:
   - Valid display name
   - Empty display name
   - Very long display name
   - Display name with special characters
3. Verify display name is required

**Expected Result**: 
- Valid display names are accepted
- Empty display name shows validation error
- Long display names are handled appropriately
- Special characters are allowed

**Priority**: Medium

### 27. Link Addition Success
**Test Case**: Test successful link addition
**Steps**:
1. Open add link modal
2. Enter valid display name
3. Enter valid URL
4. Click "Add Link" button
5. Verify link is added to folder

**Expected Result**: 
- Link is added successfully
- Modal closes automatically
- Link appears in folder with correct display name
- Link is clickable and opens in new tab

**Priority**: High

---

## Resource Management Testing

### 28. Resource Display
**Test Case**: Verify resources are displayed correctly
**Steps**:
1. Add various resources to folder:
   - Cover image
   - File upload
   - Video
   - Link
2. Verify all resources appear in folder
3. Verify resource types are clearly indicated
4. Verify resource names are displayed

**Expected Result**: 
- All resources are visible
- Resource types are clearly marked
- Names are displayed correctly
- Resources are properly organized

**Priority**: High

### 29. Resource Options Menu
**Test Case**: Test resource options menu
**Steps**:
1. Add a resource to folder
2. Click on the ellipsis (three dots) menu
3. Verify options are displayed:
   - Rename
   - Preview
   - Update File
   - Move
   - Delete
4. Test each option functionality

**Expected Result**: 
- Menu opens on click
- All options are visible and clickable
- Each option performs its intended function

**Priority**: High

### 30. Rename Resource
**Test Case**: Test resource renaming
**Steps**:
1. Add a resource to folder
2. Click ellipsis menu
3. Click "Rename" option
4. Enter new name
5. Save changes
6. Verify name is updated

**Expected Result**: 
- Rename dialog opens
- New name is saved
- Resource displays with new name
- Changes are persistent

**Priority**: Medium

### 31. Preview Resource
**Test Case**: Test resource preview functionality
**Steps**:
1. Add various resource types
2. Click "Preview" option for each type
3. Verify preview opens correctly
4. Test preview for:
   - Images
   - PDFs
   - Videos
   - Links

**Expected Result**: 
- Preview opens for supported file types
- Preview shows correct content
- Preview is properly formatted
- Preview can be closed

**Priority**: Medium

### 32. Update File
**Test Case**: Test file update functionality
**Steps**:
1. Add a file to folder
2. Click "Update File" option
3. Select new file
4. Verify file is updated
5. Test with different file types

**Expected Result**: 
- File picker opens
- New file replaces old file
- File name is updated
- Changes are saved

**Priority**: Medium

### 33. Move Resource
**Test Case**: Test resource moving functionality
**Steps**:
1. Create multiple folders
2. Add resources to one folder
3. Click "Move" option
4. Select destination folder
5. Verify resource is moved

**Expected Result**: 
- Move dialog opens
- Destination folders are listed
- Resource is moved successfully
- Resource appears in new location

**Priority**: Medium

### 34. Delete Resource
**Test Case**: Test resource deletion
**Steps**:
1. Add a resource to folder
2. Click "Delete" option
3. Confirm deletion
4. Verify resource is removed
5. Test deletion of different resource types

**Expected Result**: 
- Confirmation dialog appears
- Resource is deleted after confirmation
- Resource is removed from folder
- Deletion is permanent

**Priority**: High

---

## Client Sharing Testing

### 35. Manage Clients Access
**Test Case**: Test manage clients functionality
**Steps**:
1. Open a folder with resources
2. Click on the person icon with plus sign
3. Verify "Manage Clients" modal opens
4. Verify modal title and description

**Expected Result**: 
- Modal opens with title "Manage Clients"
- Description shows "Allows certain clients have access to this folder"
- Search field is present
- "Not shared with any clients" message is displayed

**Priority**: High

### 36. Client Search Functionality
**Test Case**: Test client search in sharing modal
**Steps**:
1. Open "Manage Clients" modal
2. Type in search field
3. Test with various search terms:
   - Client name
   - Partial name
   - Non-existent name
   - Empty search
4. Verify search results

**Expected Result**: 
- Search returns relevant results
- Partial matches work correctly
- No results message for non-existent clients
- Search is case-insensitive

**Priority**: High

### 37. Add Client to Folder
**Test Case**: Test adding client to folder
**Steps**:
1. Open "Manage Clients" modal
2. Search for a client
3. Select client from results
4. Click "Done" button
5. Verify client is added

**Expected Result**: 
- Client is added to folder
- Client appears in shared list
- "1 client" indicator is displayed
- Client name is shown correctly

**Priority**: High

### 38. Remove Client from Folder
**Test Case**: Test removing client from folder
**Steps**:
1. Add a client to folder
2. Open "Manage Clients" modal
3. Click "Remove" button next to client
4. Click "Done" button
5. Verify client is removed

**Expected Result**: 
- Client is removed from folder
- "Not shared with any clients" message appears
- Client no longer has access

**Priority**: High

### 39. Multiple Client Management
**Test Case**: Test managing multiple clients
**Steps**:
1. Add multiple clients to folder
2. Verify all clients are listed
3. Remove some clients
4. Add more clients
5. Verify client count updates

**Expected Result**: 
- All clients are displayed
- Client count is accurate
- Add/remove operations work correctly
- Changes are saved

**Priority**: Medium

---

## Folder Options Testing

### 40. Folder Options Dropdown
**Test Case**: Test folder options dropdown
**Steps**:
1. Open a folder
2. Click on "Options" dropdown
3. Verify options are displayed:
   - Rename
   - Duplicate
   - Manage clients
   - Auto Assign
   - Delete
4. Test each option

**Expected Result**: 
- Dropdown opens on click
- All options are visible
- Each option is clickable

**Priority**: High

### 41. Rename Folder
**Test Case**: Test folder renaming
**Steps**:
1. Click "Rename" option
2. Enter new folder name
3. Save changes
4. Verify name is updated
5. Test with duplicate names

**Expected Result**: 
- Rename dialog opens
- New name is saved
- Folder displays with new name
- Duplicate names are prevented

**Priority**: Medium

### 42. Duplicate Folder
**Test Case**: Test folder duplication
**Steps**:
1. Add resources to folder
2. Click "Duplicate" option
3. Verify folder is duplicated
4. Verify resources are copied
5. Verify new folder has different name

**Expected Result**: 
- Folder is duplicated successfully
- All resources are copied
- New folder has unique name
- Duplicate appears in resources list

**Priority**: Medium

### 43. Auto Assign Feature
**Test Case**: Test auto assign functionality
**Steps**:
1. Click "Auto Assign" option
2. Verify auto assign dialog opens
3. Configure auto assign settings
4. Save settings
5. Verify auto assign works

**Expected Result**: 
- Auto assign dialog opens
- Settings can be configured
- Auto assign works as configured
- Settings are saved

**Priority**: Low

### 44. Delete Folder
**Test Case**: Test folder deletion
**Steps**:
1. Add resources to folder
2. Click "Delete" option
3. Confirm deletion
4. Verify folder is deleted
5. Verify resources are also deleted

**Expected Result**: 
- Confirmation dialog appears
- Folder is deleted after confirmation
- All resources are deleted
- Folder is removed from list

**Priority**: High

---

## Cross-Browser & Device Testing

### 45. Browser Compatibility
**Test Case**: Test Resources functionality across browsers
**Steps**:
1. Test in Chrome
2. Test in Firefox
3. Test in Safari
4. Test in Edge
5. Verify all features work consistently

**Expected Result**: 
- All features work in all browsers
- UI is consistent across browsers
- No browser-specific issues

**Priority**: High

### 46. Mobile Responsiveness
**Test Case**: Test Resources on mobile devices
**Steps**:
1. Test on mobile phone
2. Test on tablet
3. Verify touch interactions work
4. Verify UI is responsive
5. Test all functionality

**Expected Result**: 
- UI adapts to mobile screens
- Touch interactions work correctly
- All features are accessible
- Performance is acceptable

**Priority**: High

### 47. Tablet Testing
**Test Case**: Test Resources on tablet devices
**Steps**:
1. Test on iPad
2. Test on Android tablet
3. Verify touch interactions
4. Verify UI scaling
5. Test all functionality

**Expected Result**: 
- UI scales appropriately
- Touch interactions work
- All features are accessible
- Performance is good

**Priority**: Medium

---

## Performance & Security Testing

### 48. File Upload Performance
**Test Case**: Test file upload performance
**Steps**:
1. Upload large files (25MB)
2. Upload multiple files simultaneously
3. Test with slow network connection
4. Monitor upload progress
5. Verify upload completion

**Expected Result**: 
- Large files upload successfully
- Multiple files upload correctly
- Progress indicators work
- Upload completes successfully

**Priority**: Medium

### 49. Security Testing
**Test Case**: Test security aspects
**Steps**:
1. Test file upload with malicious files
2. Test URL validation with malicious URLs
3. Test client access permissions
4. Test data encryption
5. Test session management

**Expected Result**: 
- Malicious files are rejected
- Malicious URLs are blocked
- Client permissions work correctly
- Data is properly encrypted
- Sessions are secure

**Priority**: High

### 50. Data Persistence
**Test Case**: Test data persistence
**Steps**:
1. Create folders and resources
2. Log out and log back in
3. Verify data is preserved
4. Test with browser refresh
5. Test with browser close/reopen

**Expected Result**: 
- All data is preserved
- Resources are accessible
- Client sharing is maintained
- No data loss occurs

**Priority**: High

---

## Edge Cases & Error Handling

### 51. Network Interruption
**Test Case**: Test behavior during network issues
**Steps**:
1. Start file upload
2. Disconnect network
3. Reconnect network
4. Verify upload resumes
5. Test with various network conditions

**Expected Result**: 
- Upload handles interruption gracefully
- Upload resumes when network returns
- Appropriate error messages shown
- No data corruption

**Priority**: Medium

### 52. Concurrent User Testing
**Test Case**: Test with multiple users
**Steps**:
1. Have multiple users access same folder
2. Test simultaneous edits
3. Test resource sharing
4. Test conflict resolution
5. Verify data consistency

**Expected Result**: 
- Multiple users can access folder
- Conflicts are handled gracefully
- Data remains consistent
- No data corruption

**Priority**: Medium

### 53. Large Dataset Testing
**Test Case**: Test with large amounts of data
**Steps**:
1. Create many folders
2. Add many resources to folders
3. Test search functionality
4. Test performance
5. Test UI responsiveness

**Expected Result**: 
- System handles large datasets
- Search remains fast
- UI remains responsive
- No performance degradation

**Priority**: Low

### 54. Error Recovery
**Test Case**: Test error recovery mechanisms
**Steps**:
1. Trigger various error conditions
2. Test error messages
3. Test recovery options
4. Test user guidance
5. Verify system stability

**Expected Result**: 
- Errors are handled gracefully
- Clear error messages shown
- Recovery options available
- System remains stable

**Priority**: Medium

---

## Test Data Requirements

### Valid Test Data
- **Folder Names**: Various valid folder names
- **File Types**: PNG, JPG, GIF, MPEG, PDF files
- **Video URLs**: Valid YouTube, Vimeo, Wistia URLs
- **Link URLs**: Valid HTTP/HTTPS URLs
- **Client Names**: Various client names for sharing

### Invalid Test Data
- **Folder Names**: Empty, too long, special characters
- **File Types**: Unsupported file types, oversized files
- **Video URLs**: Invalid URLs, non-video URLs
- **Link URLs**: Invalid formats, malicious URLs
- **Client Names**: Non-existent clients, invalid characters

---

## Success Criteria

### Functional Requirements
- All folder operations work correctly
- All resource types can be added
- Client sharing functions properly
- All options work as expected
- Data is persisted correctly

### Performance Requirements
- File uploads complete within reasonable time
- UI remains responsive during operations
- Large files are handled efficiently
- Multiple operations can run simultaneously

### Security Requirements
- File uploads are secure
- Client access is properly controlled
- Data is protected
- Malicious content is blocked

### Usability Requirements
- Interface is intuitive
- Error messages are clear
- Operations are efficient
- Mobile experience is good

---

## Conclusion

This comprehensive test suite covers all aspects of the Resources functionality, ensuring thorough testing of folder creation, resource management, client sharing, and all related features. The test cases are prioritized based on criticality and user impact, providing a structured approach to testing the Resources feature.

The test scenarios should be executed systematically, with critical functionality tested first, followed by secondary features and edge cases. Regular regression testing should be performed to ensure continued functionality as the platform evolves.
