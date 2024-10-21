
ლექცია: CSS ანიმაციები და ტრანსფორმაციები
1. ცნობა
CSS-ში ანიმაციები და ტრანსფორმაციები საშუალებას გვაძლევს ვიზუალური ეფექტები შევქმნათ ელემენტებზე. გამოყენებით @keyframes, შეგვიძლია განვსაზღვროთ, როგორ უნდა შეიცვალოს ელემენტის სტილი დროთა განმავლობაში.

2. ტრანსფორმაციები
ტრანსფორმაციის საშუალებით შეგვიძლია ელემენტების ფორმა, ზომა და პოზიცია შევცვალოთ. ძირითადი ტრანსფორმაციებია:

Transition: ელემენტის მახასიათებლების (მაგ. ფერი, ზომა) ცვლილება რბილად.
Translate: ელემენტის გადაადგილება გარკვეული ადგილიდან სხვაგან.
Rotate: ელემენტის მოვლა გარკვეული კუთხით.
Skew: ელემენტის გადახრა.
Scale: ელემენტის ზომის ცვლილება.
3. მაგალითები
3.1 Transition
html
Copy code
<!DOCTYPE html>
<html lang="ka">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Transition Example</title>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: blue;
            transition: background-color 0.5s ease;
        }
        .box:hover {
            background-color: red;
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>
3.2 Translate
html
Copy code
<!DOCTYPE html>
<html lang="ka">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Translate Example</title>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: green;
            transition: transform 0.5s ease;
        }
        .box:hover {
            transform: translateX(100px);
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>
3.3 Rotate
html
Copy code
<!DOCTYPE html>
<html lang="ka">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rotate Example</title>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: orange;
            transition: transform 0.5s ease;
        }
        .box:hover {
            transform: rotate(45deg);
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>
3.4 Skew
html
Copy code
<!DOCTYPE html>
<html lang="ka">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Skew Example</title>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: purple;
            transition: transform 0.5s ease;
        }
        .box:hover {
            transform: skew(20deg, 10deg);
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>
3.5 Scale
html
Copy code
<!DOCTYPE html>
<html lang="ka">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scale Example</title>
    <style>
        .box {
            width: 100px;
            height: 100px;
            background-color: teal;
            transition: transform 0.5s ease;
        }
        .box:hover {
            transform: scale(1.5);
        }
    </style>
</head>
<body>
    <div class="box"></div>
</body>
</html>
4. @keyframes
@keyframes საშუალებას გაწვდოს ანიმაციის სტილები სხვადასხვა დროში.

მაგალითი:
html
Copy code
<!DOCTYPE html>
<html lang="ka">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Keyframes Example</title>
    <style>
        .animate {
            width: 100px;
            height: 100px;
            background-color: pink;
            animation: move 2s infinite;
        }

        @keyframes move {
            0% { transform: translateX(0); }
            50% { transform: translateX(100px); }
            100% { transform: translateX(0); }
        }
    </style>
</head>
<body>
    <div class="animate"></div>
</body>
</html>
5. დასკვნა
CSS ანიმაციები და ტრანსფორმაციები გვეხმარება ვებსაიტების ვიზუალურ სილამაზეში და ინტერატიულობაში. ეს ინსტრუმენტები მნიშვნელოვანი კომპონენტებია თანამედროვე ვებსაიტების დიზაინის პროცესში.

თუ გაქვთ რაიმე შეკითხვა ან გაინტერესებთ კონკრეტული მაგალითები, აუცილებლად მეკითხეთ!
