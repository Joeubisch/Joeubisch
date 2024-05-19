<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tax Booking Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            width: 80%;
            margin: 0 auto;
            background: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h2 {
            text-align: center;
            color: #333;
        }
        form {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        label {
            width: 100%;
            margin-bottom: 10px;
            color: #333;
        }
        input, select, textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .form-group {
            width: 48%;
        }
        .full-width {
            width: 100%;
        }
        button {
            width: 100%;
            padding: 15px;
            background-color: #28a745;
            color: #fff;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
        }
        button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Tax Booking Form</h2>
        <form action="/submit" method="post">
            <div class="form-group">
                <label for="first-name">First Name</label>
                <input type="text" id="first-name" name="firstName" required>
            </div>
            <div class="form-group">
                <label for="last-name">Last Name</label>
                <input type="text" id="last-name" name="lastName" required>
            </div>
            <div class="form-group">
                <label for="email">Email</label>
                <input type="email" id="email" name="email" required>
            </div>
            <div class="form-group">
                <label for="phone">Phone</label>
                <input type="tel" id="phone" name="phone" required>
            </div>
            <div class="form-group full-width">
                <label for="address">Address</label>
                <input type="text" id="address" name="address" required>
            </div>
            <div class="form-group">
                <label for="city">City</label>
                <input type="text" id="city" name="city" required>
            </div>
            <div class="form-group">
                <label for="state">State</label>
                <input type="text" id="state" name="state" required>
            </div>
            <div class="form-group">
                <label for="zip">Zip Code</label>
                <input type="text" id="zip" name="zip" required>
            </div>
            <div class="form-group full-width">
                <label for="tax-type">Type of Tax Service</label>
                <select id="tax-type" name="taxType" required>
                    <option value="">Select</option>
                    <option value="personal">Personal Tax</option>
                    <option value="business">Business Tax</option>
                    <option value="other">Other</option>
                </select>
            </div>
            <div class="form-group full-width">
                <label for="details">Additional Details</label>
                <textarea id="details" name="details" rows="4"></textarea>
            </div>
            <div class="form-group full-width">
                <label for="appointment-date">Preferred Appointment Date</label>
                <input type="date" id="appointment-date" name="appointmentDate" required>
            </div>
            <div class="form-group full-width">
                <label for="appointment-time">Preferred Appointment Time</label>
                <input type="time" id="appointment-time" name="appointmentTime" required>
            </div>
            <button type="submit">Book Appointment</button>
        </form>
    </div>
</body>
</html>
