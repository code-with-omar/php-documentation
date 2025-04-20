# Chapter One: About PHP

### What is PHP and Key Points About PHP

- PHP (PHP: Hypertext Preprocessor) is a widely‑used, open‑source server‑side scripting language designed especially for web development. Here’s a high‑level overview:

1. `Origins & Name`

   - Created in 1994 by Rasmus Lerdorf.

   - Originally stood for “Personal Home Page,” now a recursive acronym: PHP: Hypertext Preprocessor.

2. `How It Works`

   i. `Server‑side:` PHP code runs on your web server.

   ii. `Embedded in HTML:` You sprinkle <?php … ?> blocks inside your HTML pages.

   iii. `Output:` The server executes the PHP, generates HTML (or JSON, XML, etc.), and sends it to the client’s browser.

3. `Common Uses`

   i. `Generating dynamic web pages` (e.g., showing user‑specific content).

   ii. `Handling form submissions and sessions` (login systems, shopping carts).

   iii.`Interacting with databases` (MySQL, PostgreSQL) to CRUD data.

   iv. `Powering content management systems` like WordPress, Drupal, Joomla.

   v. `Building RESTful APIs.`

4. Strengths

   i. `Easy to learn`—especially if you know HTML/CSS.

   ii. `Huge ecosystem:` frameworks (Laravel, Symfony), CMSs, libraries.

   iii. `Excellent database support`, especially MySQL.

   iv. `Cross‑platform:` runs on Linux, Windows, macOS.

5. Basic Syntax Example

   ```php
   <?php
     // Declare a variable
     $name = "Omar";

     // Simple function
     function greet($who) {
         return "Hello, " . htmlspecialchars($who) . "!";
     }

     // Output to browser
     echo greet($name);
   ?>

   ```

# Chapter Two: Basics PHP

### 1.1 `echo/print`

- `echo` and `print` are more or less the same. They are both used to output data to the screen.

- The differences are small: `echo` has no return value while `print` has a return value of 1 so it can be used in expressions. echo can take multiple parameters (although such usage is rare) while print can take one argument. echo is marginally faster than print.

  ```php
    // Basic symbol
    echo "Hello, World!";

    //Using echo with Multiple Parameters
    echo "Hello", " ", "World", "!";

    // Using Variables with echo:
    $name = "Alice";
    echo "Hello, $name!";

    // Concatenation with echo: You can concatenate strings using the dot (.) operator if you need more control over formatting.
    $name = "Alice";
    echo "Hello, " . $name . "!";

    // HTML in echo: echo can also output HTML tags, making it useful for dynamically generating web pages.
    echo "<h1>Welcome to My Website</h1>";

    //Good practice
    // Good practice
    echo("Hello, World!");
  ```
