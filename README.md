# Gen-Ai-101
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Crocodile Facts</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f8ff;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            text-align: center;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            margin-top: 20px;
        }

        button:hover {
            background-color: #45a049;
        }

        #factDisplay {
            margin-top: 20px;
            font-size: 18px;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Crocodile Facts</h1>
        <button id="generateFactButton">Generate Fact</button>
        <p id="factDisplay"></p>
    </div>
    <script>
        const crocodileFacts = [
            "Ancient Survivors: Crocodiles have been around for about 200 million years, making them one of the oldest living reptiles, surviving the extinction event that wiped out the dinosaurs.",
            "Powerful Bite: Crocodiles have one of the strongest bites in the animal kingdom. Their bite force can reach up to 3,700 pounds per square inch (psi).",
            "Ambush Predators: Crocodiles are excellent hunters. They often lie in wait, partially submerged in water, and ambush their prey with incredible speed and precision.",
            "Temperature-Dependent Sex Determination: The sex of crocodile hatchlings is determined by the temperature of the nest. Warmer temperatures tend to produce males, while cooler temperatures produce females.",
            "Efficient Swimmers: Crocodiles are powerful swimmers, using their tails to propel themselves through the water at speeds of up to 20 miles per hour.",
            "Long Lifespan: Crocodiles can live for a long time, with some species living up to 70 years or more in the wild.",
            "Unique Vocalizations: Crocodiles are known for their vocalizations, which include growls, hisses, and roars. They are one of the few reptiles that can communicate vocally.",
            "Protective Mothers: Female crocodiles are known to be very protective of their nests and young. They guard their eggs and often help the hatchlings reach the water after they emerge.",
            "Salt Glands: Some species of crocodiles, like the saltwater crocodile, have special glands in their tongues that help excrete excess salt, allowing them to live in saline environments.",
            "Heart Structure: Crocodiles have a unique heart with four chambers, similar to birds and mammals, which allows for efficient oxygenation of their blood, supporting their active lifestyle."
        ];

        document.getElementById('generateFactButton').addEventListener('click', function() {
            const randomIndex = Math.floor(Math.random() * crocodileFacts.length);
            const randomFact = crocodileFacts[randomIndex];
            document.getElementById('factDisplay').textContent = randomFact;
        });
    </script>
</body>
</html>
