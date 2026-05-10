<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Employee Contact Info</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #f4f4f4;
            color: #333;
            transition: background-color 0.5s ease-in-out; /* Smooth transition for body background */
        }

        /* Splash Screen Styles */
        .splash-screen {
            position: fixed; /* Covers the whole screen */
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #2874f0; /* Amazon-like blue */
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            font-size: 2em;
            z-index: 1000; /* Ensure it's on top */
            transition: opacity 1s ease-in-out; /* Fade out transition */
        }

        .splash-screen.hidden {
            opacity: 0;
            pointer-events: none; /* Make it unclickable when hidden */
        }

        .splash-screen img {
            width: 150px; /* Adjust logo size */
            margin-bottom: 10px;
        }

        .splash-screen p {
            margin: 0;
            font-weight: bold;
            font-size: 1.5em; /* Size for "BOMJ" */
            letter-spacing: 2px;
        }

        /* Main Content Styles (the table) */
        .main-content {
            width: 90%;
            max-width: 1200px; /* Max width for larger screens */
            margin: 20px auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            opacity: 0; /* Initially hidden, revealed by JS */
            transform: translateY(20px); /* Slight move down to simulate appearing */
            transition: opacity 1s ease-in-out, transform 1s ease-in-out;
        }

        .main-content.visible {
            opacity: 1;
            transform: translateY(0);
        }

        h1 {
            text-align: center;
            color: #0056b3;
            margin-bottom: 30px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }

        th, td {
            border: 1px solid #ddd;
            padding: 12px 15px;
            text-align: left;
        }

        th {
            background-color: #007bff;
            color: white;
            font-weight: bold;
        }

        tr:nth-child(even) {
            background-color: #f9f9f9;
        }

        tr:hover {
            background-color: #f1f1f1;
        }

        td:nth-child(2) { /* Style for SO CONTACT INFO column */
            white-space: nowrap; /* Prevent phone numbers from breaking */
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            .splash-screen img {
                width: 100px;
            }
            .splash-screen p {
                font-size: 1.2em;
            }
            th, td {
                padding: 8px 10px;
                font-size: 0.9em;
            }
        }
    </style>
</head>
<body>

    <!-- Splash Screen -->
    <div id="splashScreen" class="splash-screen">
        <!-- You can use an actual image tag if you have an Amazon logo URL -->
        <!-- <img src="URL_TO_YOUR_AMAZON_LOGO.png" alt="Amazon Logo"> -->
        <p>BOMJ</p>
    </div>

    <!-- Main Content (your table) -->
    <div id="mainContent" class="main-content">
        <h1>Employee Contact Information</h1>
        <table>
            <thead>
                <tr>
                    <th>NAME OF EMPLOYEE</th>
                    <th>SO CONTACT INFO</th>
                    <th>SO NAME</th>
                    <th>XPT/STORE</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Store/IN-400067-797/Mahendra_water_supply_</td>
                    <td>9833379406</td>
                    <td>MANGESH</td>
                    <td>SWEET VOICE XPT</td>
                </tr>
                <tr>
                    <td>Store/IN-400092-283/Make_My_Style_Family_Salon</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-371/Om_mobile</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-345/Expert_Security_Service</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-366/Aayush_Profile_Aluminium</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-126/Sweet_Voice_Universe</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-273/Aanya_Enterprise</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-377/Om_sai_ram_laundry_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-863/Igadget_Hub</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-386/RAJESH_COMPUTER_&_WEBSITE_SERVICES</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-768/Universal_Voice_Mobail_Shop</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-393/Shree_Haridas_decorator</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-300/MRK_Mobile_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-155/Shree_Swami_Samarth_Enterprises</td>
                    <td>9321401678</td>
                    <td>TUSAR</td>
                    <td>SWAMI SAMARTH XPT</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-728/Ramesh_Tailor</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-214/Suman_Sandwich</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400091-83/chinese_Corner</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-378/Shri_Hari_krupa_salon_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-375/Shree_Swami_samarth_optician_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-387/Rajlaxmi_Collection_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-384/Soham_Enterprises</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-149/Patel_General_Store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400091-76/R.k.Enterprises_And_Ganerel_Store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400091-87/Sai_power_loundry_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400091-77/Om_Sai_Ram_Ganeral_Store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-157/S_K_Hosiery_</td>
                    <td>8452872547</td>
                    <td>SAMEER</td>
                    <td>MAHILA</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-332/Tha_Max_Hair_Cutting_Salon</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-703/Casa_Mobile_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-708/Ayan_Real_Estate_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-773/Shah_classes_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-780/Star_mobile_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-828/Guddu_fabrication_works</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-868/K.s_classes</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-265/SS_Biryani_Center</td>
                    <td>7666824645</td>
                    <td>AKIB</td>
                    <td>SAI SALON</td>
                </tr>
                <tr>
                    <td>Store/IN-400091-65/Saivankar_Mobile_And_Computer</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-219/Sai_Salon</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-383/Shear_image_salon_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-382/Rajus_bling_salon_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-368/Shree_Swami_Samarth_Dairy_</td>
                    <td>9930396423</td>
                    <td>AARTHI</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400092-400/Multi_Mart_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-875/Harshid_Enterprises</td>
                    <td>93249 33479</td>
                    <td>CHAWDA</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-885/Raja_Chinese_Corner</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-409/Kesri_Ganeral_Store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400095-81/Vinod_General_Store</td>
                    <td>9867107838</td>
                    <td>VINOD</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400095-355/Shri_Mahavir_Prasad_Prajapati_and_general_store_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400095-62/Beauty_Queen_Parlour</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-250/Deepika_General_Store</td>
                    <td>8898633083</td>
                    <td>mahesh</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-671/Sapana_Enterprises_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-876/Lama_corner_hotel_</td>
                    <td>8169656648</td>
                    <td>noman</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-816/Shree_Laxminarayan_Ganeral_Store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-865/Shree_Bappa_Sitaram_Dairy_Farm</td>
                    <td>8005913273</td>
                    <td>SHREE BAPPA</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-881/Radhe_Krishna_Courier_Service</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-395/Craze_Tailors_&_Boutique</td>
                    <td>9004380358</td>
                    <td>RAHUL</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400092-271/Nityanand_Pan_Bidi_Shop</td>
                    <td>9137399612</td>
                    <td>PRINCE</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400103-164/Sachin_auto_garage</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400103-151/Welcome_stationery</td>
                    <td>(WA ONLY ) 9082805776</td>
                    <td>KADIR</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-903/Ganesh_electric_work</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td></td>
                    <td>9699916875</td>
                    <td>AMLESH</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-668/Mayur_Pan_Bidi_&_Cold_Drink_House</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-794/Shreeram_mobile_store</td>
                    <td>9773531234</td>
                    <td>SALIM</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-841/Nizam_Medical_And_Ganral_store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-831/Arhaan_Boutique</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-900/Royal_pipe_centre</td>
                    <td>8286427345</td>
                    <td>NITHYA</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-906/Mahalaxmi_store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-505/Ariba_Enterprises</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-809/Dheeraj_Tyres_Auto_Garage</td>
                    <td>9326773584</td>
                    <td>SANDEEP</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-798/Profesional_Hair_Cutting_Salon</td>
                    <td>9833360933</td>
                    <td>PRADEEP</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-840/Shree_salespack</td>
                    <td>9702413876</td>
                    <td>PURABJI</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-832/Om_sai_power_cleaner_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-747/Shiv_Medical_&_General_Store</td>
                    <td>9619902388</td>
                    <td>ASIF</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400095-326/Khan_imitation</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400095-359/Aaliya_imitation</td>
                    <td>885053301</td>
                    <td>FARAZ</td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400095-255/Arab_Mobail_Point</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-859/SWASTIK_ELECTRIC_AND_HARDWARE</td>
                    <td>9664617204</td>
                    <td>MUKESH</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400095-339/Beauty_Collection</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400095-366/Mobile_Adda</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-542/NARAYANKAR_&_SON'S_MUSICALS</td>
                    <td>9372070089</td>
                    <td>NIKHIL</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-616/Ignite_General_Store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-619/Punit_Enterprise</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-771/Integrity_Constructions</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-812/Citylight_Real_Estate_Advisory</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-862/M_jet_toner_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-874/J9_online_store_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-669/Ankita_Tailors</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-905/Rajesh_vadapav_center</td>
                    <td>9833022452</td>
                    <td>PARAG</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-806/Shreeji_enterprises</td>
                    <td>7208555789</td>
                    <td>SUSHEEL</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400095-371/Zaib_Kirana_store</td>
                    <td>9833609344</td>
                    <td>SAGAR</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400095-383/AS_Traders</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400092-354/Anna_samosa</td>
                    <td>7208513527</td>
                    <td>ANNA</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400092-257/C_R_Traders</td>
                    <td>7021007384</td>
                    <td>NAYAN</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400092-380/Manohar_Provision_Store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-481/Favourite_Gents_Solon</td>
                    <td>9819713773</td>
                    <td>PRITAM</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-433/Saabri_Tailor</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-820/Sheris_kitchen_</td>
                    <td>8591126041</td>
                    <td>SARVESH</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-537/Mahadev_Properties</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-748/Deepak_store</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400095-318/Jeevika_Store_</td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td>Store/IN-400067-827/Archana's_Beauty_Parlour&_Academy</td>
                    <td>8692031994</td>
                    <td>RAVINDRA</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-902/Sk_Enterprises</td>
                    <td>7738243924</td>
                    <td>SHYAM</td>
                    <td>STORE</td>
                </tr>
                <tr>
                    <td>Store/IN-400067-722/Kismat_Laundry</td>
                    <td>8169801808</td>
                    <td>SUNIL</td>
                    <td>STORE</td>
                </tr>
            </tbody>
        </table>
    </div>

    <script>
        // Select the splash screen and the main content
        const splashScreen = document.getElementById('splashScreen');
        const mainContent = document.getElementById('mainContent');

        // Function to hide the splash screen and show the main content
        function showContent() {
            // Add the 'hidden' class to fade out the splash screen
            splashScreen.classList.add('hidden');
            // Add the 'visible' class to fade in and move up the main content
            mainContent.classList.add('visible');
            // Optional: Change body background after transition for a smoother feel
            setTimeout(() => {
                document.body.style.backgroundColor = '#ffffff'; // Or your preferred final background
            }, 1000); // Match the duration of the splash screen fade-out
        }

        // Set a timeout to call showContent after 3 seconds (3000 milliseconds)
        // You can adjust this duration as needed
        setTimeout(showContent, 3000);
    </script>

</body>
</html>
