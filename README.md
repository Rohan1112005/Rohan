<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Parking Slot Booking System</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Login Page -->
    <div id="login">
        <h2>Login</h2>
        <form id="loginForm" onsubmit="return checkLogin()">
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" required>
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" required>
            <button type="submit">Login</button>
        </form>
    </div>

    <!-- Car Parking Slot Booking Page -->
    <div id="bookingPage" style="display:none;">
        <h2>Book Your Parking Slot</h2>
        <form id="bookingForm">
            <label>Select Slots:</label>
            <div>
                <input type="checkbox" id="slot1" name="slot" value="Slot 1">
                <label for="slot1">Slot 1</label>
            </div>
            <div>
                <input type="checkbox" id="slot2" name="slot" value="Slot 2">
                <label for="slot2">Slot 2</label>
            </div>
            <div>
                <input type="checkbox" id="slot3" name="slot" value="Slot 3">
                <label for="slot3">Slot 3</label>      
            </div>
            <div>
                <input type="checkbox" id="slot4" name="slot" value="Slot 4">
                <label for="slot4">Slot 4</label>
            </div>

            <label for="duration">Duration (hours):</label>
            <input type="number" id="duration" name="duration" min="1" required>

            <button type="button" onclick="confirmBooking()">Confirm Booking</button>
        </form>

        <div id="confirmationMessage" style="display:none;">
            <h3>Booking Confirmed!</h3>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
