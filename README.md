# imgupld
File image to exploit Unrestricted File Upload or File Upload Attack vulnerability

<img width="200" height="150 alt="ponep" src="https://github.com/samphoerna/imgupld/assets/139729508/7866dcaa-fa51-4aef-ae32-6a51d354d329">

---

**Exploit:**

The exploit involves bypassing any client-side or server-side file type checks to upload malicious files. Attackers can change the file extension, forge the MIME type, or use encoding techniques to disguise the malicious content as legitimate files. Once the malicious file is uploaded, attackers can then execute code remotely, escalate privileges, deface the website, or compromise user data.

**How it works:**

1. The web application provides a file upload functionality without proper file type checking.
2. The attacker identifies the file upload vulnerability and attempts to upload a malicious file.
3. The attacker changes the file extension or manipulates the MIME type to bypass any existing checks.
4. The server accepts the malicious file, saving it in a publicly accessible directory or processing it on the server.
5. The attacker can now execute the uploaded script or take control over the application and server.

**Mitigations for File Upload Vulnerabilities:**

- File Validation: Implement strict validation on file uploads, including checking file extensions, MIME types, and content to ensure they match the expected file type.
- Server-Side Validation: Perform file validation on the server-side, regardless of any client-side checks.
- Restricted File Upload Directory: Store uploaded files in a directory with limited permissions, restricting access to the uploaded files.
- Rename Uploaded Files: Use a unique name for the uploaded files to avoid potential conflicts and prevent overwriting critical files.
- Content Disposition: Set the Content-Disposition header to "attachment" to prevent browsers from displaying uploaded files inline.
- Implementing CAPTCHA or CSRF Protection: Add CAPTCHA or CSRF protection to prevent automated attacks and unauthorized uploads.
- Use a Secure File Upload Library: Consider using a well-tested, secure file upload library that handles file uploads with built-in security measures.

---
==Before Use==

change extensions to PHP or rename file after uploads

this is still prototype, im never use it yet
