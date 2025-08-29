<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Enhanced HTML5 Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      line-height: 1.6;
    }
    header, footer {
      background: #f4f4f4;
      padding: 10px;
    }
    main {
      margin-top: 20px;
    }
    form {
      max-width: 600px;
      background: #fafafa;
      padding: 15px;
      border: 1px solid #ccc;
      border-radius: 8px;
    }
    label {
      display: block;
      margin-top: 10px;
    }
    input, select, textarea, button {
      width: 100%;
      padding: 8px;
      margin-top: 4px;
    }
    table {
      border-collapse: collapse;
      width: 100%;
      margin-top: 20px;
    }
    table, th, td {
      border: 1px solid #ccc;
      padding: 8px;
    }
    img {
      max-width: 100%;
    }
  </style>
</head>
<body>

  <header>
    <h1>Enhanced HTML5 Form Example</h1>
    <p>This page demonstrates semantic HTML, form validation, media elements, tables, and lists.</p>
  </header>

  <main>
    <section aria-labelledby="form-section">
      <h2 id="form-section">User Registration Form</h2>
      <form action="/submit" method="post" autocomplete="on" novalidate>
        
        <!-- Personal Info -->
        <label for="fullname">Full Name *</label>
        <input type="text" id="fullname" name="fullname" placeholder="Jane Doe" required>

        <label for="email">Email *</label>
        <input type="email" id="email" name="email" placeholder="jane@example.com" required>

        <label for="password">Password *</label>
        <input type="password" id="password" name="password" minlength="6" required>

        <label for="dob">Date of Birth</label>
        <input type="date" id="dob" name="dob">

        <label for="phone">Phone Number</label>
        <input type="tel" id="phone" name="phone" placeholder="123-456-7890" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}">

        <!-- Preferences -->
        <label for="country">Country</label>
        <select id="country" name="country">
          <option value="">-- Select a country --</option>
          <option value="us">United States</option>
          <option value="uk">United Kingdom</option>
          <option value="ca">Canada</option>
        </select>

        <label>
          <input type="checkbox" name="subscribe" checked>
          Subscribe to newsletter
        </label>

        <label>Gender</label>
        <label><input type="radio" name="gender" value="female"> Female</label>
        <label><input type="radio" name="gender" value="male"> Male</label>
        <label><input type="radio" name="gender" value="other"> Other</label>

        <label for="bio">Short Bio</label>
        <textarea id="bio" name="bio" rows="4" placeholder="Tell us about yourself..."></textarea>

        <!-- Readonly Example -->
        <label for="referral">Referral Code</label>
        <input type="text" id="referral" name="referral" value="REF12345" readonly>

        <button type="submit">Submit</button>
      </form>
    </section>

    <section aria-labelledby="info-section">
      <h2 id="info-section">Additional Information</h2>

      <!-- List -->
      <h3>Benefits of Registering:</h3>
      <ul>
        <li>Access to exclusive content</li>
        <li>Monthly newsletters</li>
        <li>Free downloadable resources</li>
      </ul>

      <!-- Table -->
      <h3>Pricing Table</h3>
      <table>
        <thead>
          <tr>
            <th>Plan</th>
            <th>Price</th>
            <th>Features</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Basic</td>
            <td>$0</td>
            <td>Access to free articles</td>
          </tr>
          <tr>
            <td>Pro</td>
            <td>$9.99/mo</td>
            <td>Premium content & support</td>
          </tr>
          <tr>
            <td>Enterprise</td>
            <td>$29.99/mo</td>
            <td>Team access & analytics</td>
          </tr>
        </tbody>
      </table>
    </section>

    <!-- Media Section -->
    <section aria-labelledby="media-section">
      <h2 id="media-section">Media Samples</h2>
      <figure>
        <img src="https://via.placeholder.com/600x200" alt="Sample Banner">
        <figcaption>Sample image for layout demonstration</figcaption>
      </figure>

      <audio controls>
        <source src="sample-audio.mp3" type="audio/mp3">
        Your browser does not support the audio element.
      </audio>

      <video controls width="100%" height="auto">
        <source src="sample-video.mp4" type="video/mp4">
        Your browser does not support the video element.
      </video>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Enhanced Form Demo. All rights reserved.</p>
  </footer>

</body>
</html>
