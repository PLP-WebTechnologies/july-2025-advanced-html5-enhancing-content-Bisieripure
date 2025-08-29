<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Enhanced HTML5 Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 2em;
      background-color: #f9f9f9;
    }
    header, main, footer {
      max-width: 800px;
      margin: auto;
    }
    form {
      background: #fff;
      padding: 1.5em;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    fieldset {
      margin-bottom: 1em;
      border: 1px solid #ccc;
      padding: 1em;
    }
    legend {
      font-weight: bold;
    }
    label {
      display: block;
      margin-top: 0.5em;
    }
    input, select, textarea {
      width: 100%;
      padding: 0.5em;
      margin-top: 0.2em;
      box-sizing: border-box;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 1em;
    }
    th, td {
      border: 1px solid #ccc;
      padding: 0.5em;
      text-align: left;
    }
    ul {
      margin-top: 1em;
    }
    img {
      max-width: 100%;
      height: auto;
      margin-top: 1em;
    }
  </style>
</head>
<body>
  <header>
    <h1>Enhanced HTML5 Form</h1>
    <p>This page demonstrates a well-structured HTML5 form with semantic layout, validation, and multimedia elements.</p>
  </header>

  <main>
    <section>
      <h2>Features Overview</h2>
      <ul>
        <li>Semantic HTML layout</li>
        <li>Form with diverse input types</li>
        <li>HTML5 validation and accessibility</li>
        <li>Tables and media integration</li>
      </ul>
    </section>

    <section>
      <h2>Sample Data Table</h2>
      <table>
        <thead>
          <tr>
            <th>Name</th>
            <th>Role</th>
            <th>Email</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Aiko Tanaka</td>
            <td>Designer</td>
            <td>aiko@example.com</td>
          </tr>
          <tr>
            <td>James Mwangi</td>
            <td>Developer</td>
            <td>james@example.com</td>
          </tr>
        </tbody>
      </table>
    </section>

    <section>
      <h2>Embedded Media</h2>
      <img src="https://via.placeholder.com/600x200?text=Sample+Banner" alt="Sample banner image" />
      <p>Below is a sample video embedded using HTML5:</p>
      <video controls width="100%">
        <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4" />
        Your browser does not support the video tag.
      </video>
    </section>

    <section>
      <h2>Registration Form</h2>
      <form action="/submit" method="POST" autocomplete="on">
        <fieldset>
          <legend>Personal Information</legend>
          <label for="fullname">Full Name:</label>
          <input type="text" id="fullname" name="fullname" placeholder="John Doe" required />

          <label for="email">Email:</label>
          <input type="email" id="email" name="email" placeholder="you@example.com" required />

          <label for="dob">Date of Birth:</label>
          <input type="date" id="dob" name="dob" required />

          <label for="gender">Gender:</label>
          <select id="gender" name="gender" required>
            <option value="">--Select--</option>
            <option value="female">Female</option>
            <option value="male">Male</option>
            <option value="other">Other</option>
          </select>
        </fieldset>

        <fieldset>
          <legend>Account Details</legend>
          <label for="username">Username:</label>
          <input type="text" id="username" name="username" placeholder="Choose a username" required minlength="4" maxlength="15" />

          <label for="password">Password:</label>
          <input type="password" id="password" name="password" required minlength="6" />

          <label for="confirm">Confirm Password:</label>
          <input type="password" id="confirm" name="confirm" required minlength="6" />
        </fieldset>

        <fieldset>
          <legend>Preferences</legend>
          <label for="bio">Short Bio:</label>
          <textarea id="bio" name="bio" rows="4" placeholder="Tell us about yourself..."></textarea>

          <label for="newsletter">Subscribe to newsletter:</label>
          <input type="checkbox" id="newsletter" name="newsletter" />

          <label for="readonly-info">Referral Code (readonly):</label>
          <input type="text" id="readonly-info" name="referral" value="REF12345" readonly />
        </fieldset>

        <button type="submit">Submit</button>
        <button type="reset">Reset</button>
      </form>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Enhanced Form Demo. All rights reserved.</p>
  </footer>
</body>
</html>

