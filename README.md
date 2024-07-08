<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Department Registration Form - KITSW</title>
    <style>
        body {
            font-family: 'Helvetica Neue', sans-serif;
            background-color: #f0f4f8;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            min-height: 100vh;
        }
        .container {
            width: 90%;
            max-width: 800px;
            text-align: center;
            padding: 20px;
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.1);
            margin: 20px;
        }
        .title-1 {
            color: #ffffff;
            font-size: 28px;
            background-color: #0077b6;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
        }
        .add {
            font-size: 16px;
            margin-top: 10px;
            color: #d1e8e2;
        }
        .marque-container {
            background-color: #ffffff;
            padding: 10px 20px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            width: 95%;
            text-align: center;
            margin-top: 20px;
        }
        marquee {
            font-size: 20px;
            color: #e63946;
        }
        .info {
            background-color: #ffffff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            width: 95%;
            text-align: center;
            margin-top: 20px;
            font-size: 18px;
            color: #333333;
        }
        form {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .form-field {
            width: 100%;
            max-width: 600px;
            background-color: #ffffff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
        }
        label {
            margin-bottom: 10px;
            font-size: 16px;
            color: #0077b6;
            text-align: left;
            display: block;
        }
        input, select {
            padding: 12px;
            width: calc(100% - 24px);
            border: 1px solid #ced4da;
            border-radius: 5px;
            font-size: 16px;
            margin-bottom: 10px;
        }
        button {
            padding: 12px 24px;
            font-size: 18px;
            color: #ffffff;
            background-color: #0077b6;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
            margin-top: 20px;
        }
        button:hover {
            background-color: #005f8b;
            transform: translateY(-2px);
        }
        /* Checkbox Styling */
        .checkbox-group {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-top: 10px;
        }
        .checkbox-item {
            width: 45%;
            margin-bottom: 10px;
        }
        .checkbox-item label {
            display: inline-block;
            vertical-align: middle;
            margin-left: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="title-1">
            <h1>KAKATIYA INSTITUTE OF TECHNOLOGY AND SCIENCE</h1>
            <p class="add">Near Kitsw Point, Warangal, Telangana, 506015</p>
        </div>
        <div class="marque-container">
            <marquee>Welcome to the Department Registration Form for KITSW. Please fill out the form below to register.</marquee>
        </div>
        <div class="info">
            <p>Admission to Kakatiya Institute of Technology and Science (KITSW) is based on ranks achieved in the EAMCET exam. The process includes rank calculation, counseling registration, choice filling, and seat allotment. Students with higher ranks have better chances of securing their desired courses. Successful candidates must complete document verification and fee payment to confirm their admission. Stay updated with official notifications for a smooth admission experience.</p>
        </div>
        <br>
        <form action="https://kitsw.ac.in/register" method="post">
            <div class="form-field">
                <label for="name">Full Name</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>
            </div>
            <div class="form-field">
                <label for="care">Full Name Of Parents/Guardian</label>
                <input type="text" id="care" name="care" placeholder="Enter Your Parent/Guardian Name" required>
            </div>
            <div class="form-field">
                <label for="gender">Gender</label>
                <select id="gender" name="gender" required>
                    <option value="">Select Gender</option>
                    <option value="male">Male</option>
                    <option value="female">Female</option>
                    <option value="other">Other</option>
                </select>
            </div>
            <div class="form-field">
                <label for="email">Email</label>
                <input type="email" id="email" name="email" placeholder="Enter Your Email Id" required>
            </div>
            <div class="form-field">
                <label for="contact">Contact Number</label>
                <input type="text" id="contact" name="contact" placeholder="Enter Your Contact Details" required>
            </div>
            <div class="form-field">
                <label>Select Departments</label>
                <br>
                <div class="checkbox-group">
                    <div class="checkbox-item">
                        <input type="checkbox" id="cse" name="department[]" value="CSE">
                        <label for="cse">Computer Science and Engineering</label>
                    </div>
                    <div class="checkbox-item">
                        <input type="checkbox" id="ece" name="department[]" value="ECE">
                        <label for="ece">Electronics and Communication Engineering</label>
                    </div>
                    <div class="checkbox-item">
                        <input type="checkbox" id="eee" name="department[]" value="EEE">
                        <label for="eee">Electrical and Electronics Engineering</label>
                    </div>
                    <div class="checkbox-item">
                        <input type="checkbox" id="me" name="department[]" value="ME">
                        <label for="me">Mechanical Engineering</label>
                    </div>
                    <div class="checkbox-item">
                        <input type="checkbox" id="ce" name="department[]" value="CE">
                        <label for="ce">Civil Engineering</label>
                    </div>
                </div>
            </div>
            <div class="form-field">
                <label for="rank">EAMCET Rank</label>
                <input type="text" id="rank" name="rank" placeholder="Enter Your EAMCET Rank" required>
            </div>
            <button type="submit">Submit</button>
        </form>
    </div>
</body>
</html>
