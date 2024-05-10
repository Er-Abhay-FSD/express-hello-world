# Interview Questions and Answers

## Basic Concepts

1. **You change a state? Is it a library or framework?**
   React.js is a JavaScript library for building user interfaces, including the ability to change state and handle UI updates efficiently through components.

2. **What are components in React.js?**
   Components are reusable and independent building blocks in React that encapsulate logic and UI elements. They can be either functional components or class components.

3. **What is virtual DOM in React?**
   The virtual DOM is a lightweight copy of the actual DOM in memory. React uses it to perform efficient DOM updates by first making changes to the virtual DOM and then reconciling those changes with the real DOM.

4. **What is JSX? How JSX is parsed into JavaScript?**
   JSX is a syntax extension for JavaScript that allows you to write HTML-like code within JavaScript. JSX is transformed into regular JavaScript function calls by tools like Babel during the build process.

5. **What is the use of Webpack?**
   Webpack is a module bundler for JavaScript applications. It bundles all the modules and assets of an application into static files for deployment, optimizing performance and enabling features like code splitting and hot module replacement.

6. **Suppose a website is very fast, and I'm willing to make it slow. What actions could be taken?**
   Introducing delays in server responses, increasing image sizes, adding unnecessary scripts or styles, and reducing caching efficiency are some actions that could make a website slower deliberately.

7. **What is CDN? How does CDN work?**
   A Content Delivery Network (CDN) is a network of distributed servers that deliver web content to users based on their geographic locations. CDN caches content at edge servers closest to users, reducing latency and improving website performance.

8. **What is Indexing in Database? Do Indexing affect only fetching, or will it affect insertion and updation also?**
   Indexing in a database involves creating data structures to quickly locate and access rows in a table. While indexing primarily improves fetching performance, it can also affect insertion and updating operations by adding overhead due to maintaining the index structures.

9. **How will you move a commit from one branch to another branch?**
   You can move a commit from one branch to another using `git cherry-pick` or by using `git rebase -i` to interactively rebase commits onto another branch.

10. **What does git stash command do?**
    The `git stash` command temporarily shelves changes in your working directory, allowing you to switch to another branch or apply the changes later.

11. **Which website will be faster, the one built with JavaScript or the one built with React?**
    Both JavaScript and React can be used to build fast websites. React is a JavaScript library for building UI components efficiently, so a website built with React can be fast if it's well-optimized.

12. **What actions could be taken to make a website faster?**
    Actions to make a website faster include optimizing images, minimizing HTTP requests, leveraging browser caching, using a CDN, minimizing render-blocking scripts and stylesheets, and employing techniques like lazy loading and code splitting.

13. **Where session data is stored in backend servers?**
    Session data is typically stored on the server-side, either in memory, a database, or a dedicated session store like Redis or Memcached.

14. **Git stores all the data in which folder?**
    Git stores all its data in a hidden directory called `.git` within the root directory of a Git repository.

15. **How does the gitignore file work?**
    The `.gitignore` file specifies intentionally untracked files that Git should ignore. It uses glob patterns to match files and directories that should not be committed to the repository.

16. **How to verify an email? Which is the best method to verify the email, client-based, or server-based?**
    Email verification typically involves sending a confirmation link to the email address provided by the user. Server-side verification is generally considered more secure and reliable than client-side verification, as it ensures that the email actually exists and is under the user's control.

17. **Will a session work if we decline cookies?**
    Sessions can still work even if cookies are declined by using other methods of session management, such as URL rewriting or hidden form fields. However, relying solely on cookies for session management is the most common approach.

18. **When reopening a website after closing it, session made on that website gets destroyed automatically, and you need to log in again. Why so?**
    This behavior occurs because the session cookie, which identifies the user's session, is typically set to expire when the browser is closed. When the browser is reopened, the session cookie is no longer valid, leading to the loss of the session state.

19. **What is GitHub's cherry-pick command?**
    GitHub does not have a cherry-pick command; however, Git, which is the version control system used by GitHub, has a `git cherry-pick` command. This command allows you to apply a specific commit from one branch to another.

20. **What is DOM?**
    The Document Object Model (DOM) is a programming interface for web documents. It represents the structure of an HTML or XML document as a tree of objects that can be manipulated and accessed programmatically.

21. **What is encryption and decryption? What is hashing? What is the purpose of salting?**
    Encryption is the process of converting plaintext into ciphertext to secure it from unauthorized access, while decryption is the reverse process. Hashing is the transformation of input data into a fixed-size string of characters using a hash function. Salting involves adding random data to input before hashing to prevent attacks like rainbow tables and dictionary attacks.

22. **How JWT works? How do symmetric and asymmetric algorithms work? What are different algorithms for encryption and hashing?**
    JSON Web Tokens (JWT) are used for securely transmitting information between parties as a JSON object. Symmetric algorithms use the same key for both encryption and decryption, while asymmetric algorithms use different keys for encryption and decryption. Common encryption algorithms include AES and RSA, while hashing algorithms include MD5, SHA-1, and SHA-256.

23. **Do all hashing algorithms generate a hash value of fixed-size string of characters?**
    No, not all hashing algorithms generate hash values of fixed sizes. Some hashing algorithms produce fixed-size output, while others can produce variable-length output.

24. **Can there be two computers with the same public IP?**
    Yes, multiple computers can share the same public IP address, especially in cases where they are behind a NAT (Network Address Translation) router.

25. **How does a router assign IP addresses to computers? What happens when you hit a URL when you are connected with a router?**
    Routers typically use DHCP (Dynamic Host Configuration Protocol) to assign IP addresses to

## Scenario-Based Questions

### Q1: How will you build a YouTube-like automatic video quality controller without using any JavaScript library?
   * Approach: Determine network latency using various methods such as ping or HTTP requests. Based on the latency, switch between different video qualities using HTML5 video element attributes or JavaScript to dynamically adjust the video source URL.

### Q2: How will you implement an OTP verification tool without using backend?
   * Approach: Generate a one-time password (OTP) client-side using JavaScript. Send the OTP to the user's email or mobile number. Allow the user to enter the OTP on the frontend and validate it locally without backend interaction.

### Q3: Suppose there is an elevator, and a person is standing on the 6th floor, another person is standing on the 10th floor, then how will it work, and what can be the algorithm and data structure used in the working of the elevator?
   * Approach: Use an algorithm like the Shortest Seek Time First (SSTF) or First Come First Serve (FCFS) to determine the elevator's movement. Implement a queue data structure to manage the requests for each floor, and update the elevator's direction and destination based on the current and requested floors.

