<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tech & Network Blog</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      color: #333;
    }

    header {
      background: #1a1a2e;
      color: #fff;
      padding: 1.5rem 0;
      text-align: center;
    }

    header h1 {
      margin: 0;
      font-size: 2.5rem;
    }

    header p {
      margin: 0.5rem 0 0;
      font-size: 1.2rem;
    }

    nav {
      background: #162447;
      text-align: center;
      padding: 0.5rem 0;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
    }

    nav a:hover {
      text-decoration: underline;
    }

    main {
      padding: 2rem;
    }

    .blog-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 2rem;
    }

    .blog-card {
      background: #fff;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      width: 300px;
      padding: 1.5rem;
      text-align: left;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .blog-card:hover {
      transform: scale(1.05);
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }

    .blog-card h3 {
      margin-top: 0;
      color: #1a1a2e;
    }

    .blog-card p {
      margin: 0.5rem 0 1rem;
      color: #555;
    }

    .blog-card a {
      color: #1a1a2e;
      text-decoration: none;
      font-weight: bold;
    }

    .blog-card a:hover {
      text-decoration: underline;
    }

    footer {
      background: #1a1a2e;
      color: #fff;
      text-align: center;
      padding: 1rem 0;
      margin-top: 2rem;
    }

    /* Contact Page Styles */
    #contact {
      background: #f7f7f7;
      padding: 60px 0;
    }

    .section-header h3 {
      text-align: center;
      font-size: 36px;
      font-weight: 500;
      padding-bottom: 20px;
    }

    .section-header p {
      text-align: center;
      font-size: 18px;
      margin-top: 0;
      color: #666;
    }

    .contact-info {
      text-align: center;
    }

    .contact-info .contact-address, .contact-info .contact-phone, .contact-info .contact-email {
      margin-bottom: 20px;
    }

    .contact-info i {
      font-size: 32px;
      color: #18d26e;
    }

    .contact-info h3 {
      font-size: 20px;
      margin: 10px 0;
    }

    .contact-form .form-control {
      margin-bottom: 20px;
    }

    .form button {
      background: #18d26e;
      border: 0;
      padding: 10px 30px;
      color: #fff;
      transition: 0.4s;
    }

    .form button:hover {
      background: #14a359;
    }

    .validation {
      color: red;
      font-size: 12px;
    }

    #sendmessage, #errormessage {
      display: none;
      text-align: center;
      padding: 10px;
      margin-bottom: 15px;
    }

    #sendmessage {
      color: green;
    }

    #errormessage {
      color: red;
    }
  </style>
</head>
<body>
  <header>
    <h1>Tech & Network Blog</h1>
    <p>Insights, Tutorials, and Updates from the World of Technology</p>
  </header>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a> <!-- Added Contact link -->
  </nav>
  <main>
    <h2>Latest Blogs</h2>
    <div class="blog-container">
      <div class="blog-card">
        <h3>Understanding Network Protocols</h3>
        <p>A deep dive into the essential protocols powering the internet.</p>
        <a href="network-protocols.html">Read More</a>
      </div>
      <div class="blog-card">
        <h3>System Administration Tips</h3>
        <p>Best practices to optimize your infrastructure and workflows.</p>
        <a href="system-admin-tips.html">Read More</a>
      </div>
      <div class="blog-card">
        <h3>Cloud Computing Trends</h3>
        <p>Explore the future of cloud-based technology in modern IT.</p>
        <a href="cloud-trends.html">Read More</a>
      </div>
    </div>
  </main>

  <!-- Contact Section -->
  <section id="contact">
    <div class="container">
      <div class="section-header">
        <h3>Contact Us</h3>
        <p>We’d love to hear from you! Send us a message below.</p>
      </div>

      <div class="row contact-info">
        <div class="col-md-4">
          <div class="contact-address">
            <i class="fa fa-map-marker"></i>
            <h3>Address</h3>
            <address>A108 Your address, Dhaka</address>
          </div>
        </div>
        <div class="col-md-4">
          <div class="contact-phone">
            <i class="fa fa-phone"></i>
            <h3>Phone Number</h3>
            <p><a href="tel:+8801748419892">+880 174 8419892</a></p>
          </div>
        </div>
        <div class="col-md-4">
          <div class="contact-email">
            <i class="fa fa-envelope"></i>
            <h3>Email</h3>
            <p><a href="mailto:aradbin@gmail.com">aradbin@gmail.com</a></p>
          </div>
        </div>
      </div>

      <div class="form">
        <div id="sendmessage">Your message has been sent. Thank you!</div>
        <div id="errormessage"></div>
        <form action="" method="post" role="form" class="contactForm">
          <div class="form-row">
            <div class="form-group col-md-6">
              <input type="text" name="name" class="form-control" id="name" placeholder="Your Name" />
              <div class="validation" id="name-error"></div>
            </div>
            <div class="form-group col-md-6">
              <input type="email" class="form-control" name="email" id="email" placeholder="Your Email" />
              <div class="validation" id="email-error"></div>
            </div>
          </div>
          <div class="form-row">
            <div class="form-group col-md-6">
              <input type="text" class="form-control" name="mobile" id="mobile" placeholder="Your Mobile Number" />
              <div class="validation" id="mobile-error"></div>
            </div>
            <div class="form-group col-md-6">
              <input type="text" class="form-control" name="subject" id="subject" placeholder="Subject" />
              <div class="validation" id="subject-error"></div>
            </div>
          </div>
          <div class="form-group">
            <textarea class="form-control" name="message" rows="5" placeholder="Message"></textarea>
            <div class="validation" id="message-error"></div>
          </div>
          <div class="text-center">
            <button type="submit">Send Message</button>
          </div>
        </form>
      </div>
    </div>
  </section>

  <footer>
    <p>&copy; 2024 Tech & Network Blog. All rights reserved.</p>
  </footer>

  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
  <script>
    // Contact form validation
    $(document).ready(function() {
      $(".contactForm").on("submit", function(e) {
        e.preventDefault();
        var isValid = true;

        // Validate name
        if ($("#name").val() == "") {
          $("#name-error").text("Please enter your name.");
          isValid = false;
        } else {
          $("#name-error").text("");
        }

        // Validate email
        if ($("#email").val() == "") {
          $("#email-error").text("Please enter your email.");
          isValid = false;
        } else {
          $("#email-error").text("");
        }

        // Validate mobile
        if ($("#mobile").val() == "") {
          $("#mobile-error").text("Please enter your mobile number.");
          isValid = false;
        } else {
          $("#mobile-error").text("");
        }

        // Validate subject
        if ($("#subject").val() == "") {
          $("#subject-error").text("Please enter the subject.");
          isValid = false;
        } else {
          $("#subject-error").text("");
        }

        // Validate message
        if ($("#message").val() == "") {
          $("#message-error").text("Please enter your message.");
          isValid = false;
        } else {
          $("#message-error").text("");
        }

        // Submit form if valid
        if (isValid) {
          $("#sendmessage").show();
          $("#errormessage").hide();
        } else {
          $("#sendmessage").hide();
          $("#errormessage").show().text("Please fill out all fields.");
        }
      });
    });
  </script>
</body>
</html>
