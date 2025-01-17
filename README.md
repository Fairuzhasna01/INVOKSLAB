/* General reset for body and html */
html, body {
    margin: 0; /* Reset default margin */
    padding: 0; /* Reset default padding */
    width: 100%; /* Ensure full width */
    overflow-x: hidden; /* Prevent horizontal scrolling */
}
body {
    font-family: 'Roboto', sans-serif;
    background-color: #f3f4f6; /* bg-gray-100 */
}
.header-gradient {
    background: linear-gradient(to right, #009b4c, #f08519, #2f318b);
    color: white;
    padding: 1rem; /* p-4 */
}
.container {
    max-width: 1200px; /* Set a max width for the container */
    margin: 0 auto; /* Center the container */
    padding: 0 15px; /* Add horizontal padding */
}

/* Slider styles */
.slider {
    display: flex;
    width: 80%; /* Lebih lebar untuk menampung gambar dan duplikatnya */
    height: 120%;
    animation: slideAnimation 18s infinite; /* Durasi total animasi diatur lebih lama untuk perulangan yang mulus */
}


/* Animasi bergerak maju satu per satu */
@keyframes slideAnimation {
    0% {
        transform: translateX(0); /* Gambar pertama muncul */
    }
    16.66% {
        transform: translateX(-16.66%); /* Gambar kedua muncul */
    }
    33.33% {
        transform: translateX(-33.33%); /* Gambar ketiga muncul */
    }
    50% {
        transform: translateX(-50%); /* Gambar pertama duplikat muncul */
    }
    66.66% {
        transform: translateX(-66.66%); /* Gambar kedua duplikat muncul */
    }
    83.33% {
        transform: translateX(-83.33%); /* Gambar ketiga duplikat muncul */
    }
    100% {
        transform: translateX(0); /* Kembali ke gambar pertama tanpa mundur */
    }
}
.laboratory-image {
    height: 200px; /* Set a fixed height */
    object-fit: cover; /* Maintain aspect ratio and cover the area */
    width: 100%; /* Ensure full width */
}

/* Button styles */
.slider-button {
    position: absolute; /* Positions the buttons relative to the slider-container */
    top: 50%; /* Vertically centers the buttons */
    transform: translateY(-50%); /* Adjusts the position to truly center the buttons */
    background-color: rgba(0, 0, 0, 0.5); /* Semi-transparent black background */
    color: white; /* White text color for the buttons */
    border: none; /* Removes default border */
    padding: 10px; /* Adds padding around the buttons */
    cursor: pointer; /* Changes cursor to pointer on hover */
}

.slider-button.prev {
    left: 10px; /* Positions the previous button on the left */
}

.slider-button.next {
    right: 10px; /* Positions the next button on the right */
}
/* introduction */

body {
    font-family: Arial, sans-serif; /* Default font for the body */
    margin: 0;
    padding: 0;
}

.py-8 {
    padding-top: 2rem; /* Padding for the top */
    padding-bottom: 2rem; /* Padding for the bottom */
}

.bg-gradient {
    background: linear-gradient(to right, #4a90e2, #9013fe); /* Gradient background for the about section */
    position: relative; /* Positioning context for absolute elements */
    overflow: hidden; /* Hide overflow */
}

.bg-gradient::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-image: url('background-pattern.png'); /* Optional background pattern */
    opacity: 0.1; /* Faint background pattern */
    z-index: 1; /* Place behind text */
}

.container {
    max-width: 1200px; /* Max width for container */
    margin-left: auto;
    margin-right: auto;
    padding-left: 1rem; /* Padding for left */
    padding-right: 1rem; /* Padding for right */
    position: relative; /* Positioning context for text layering */
    z-index: 2; /* Ensure text is above background */
}

.text-center {
    text-align: center; /* Center text */
}

.text-white {
    color: white; /* White text color */
}

.text-blue-900 {
    color: #1e3a8a; /* Dark blue color for headings */
}

.bg-gray-200 {
    background-color: #E5E7EB; /* Light gray background for the vision and mission section */
}

.shadow-md {
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Medium shadow for the card */
}

.rounded-lg {
    border-radius: 0.5rem; /* Rounded corners for the card */
}

.btn-primary {
    display: inline-block;
    padding: 0.5rem 1.5rem; /* Padding for the button */
    background-color: #007bff; /* Button background color */
    color: white; /* Button text color */
    border-radius: 5px; /* Rounded corners for the button */
    text-decoration: none; /* No underline */
    font-weight: bold; /* Bold text */
    transition: background-color 0.3s ease; /* Smooth transition for background color */
}

.btn-primary:hover {
    background-color: #0056b3; /* Darker shade on hover */
}

.transform {
    transition: transform 0.3s ease; /* Smooth transition for transform effects */
}

.hover\:scale-105:hover {
    transform: scale(1.05); /* Scale effect on hover */
}

.hover\:shadow-lg:hover {
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2); /* Shadow effect on hover */
}

/*vision mission*/

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

.py-8 {
    padding-top: 2rem;
    padding-bottom: 2rem;
}

.bg-gray-200 {
    background-color: #E5E7EB; /* Light gray background for the vision and mission section */
}

.container {
    max-width: 1200px;
    margin-left: auto;
    margin-right: auto;
    padding-left: 1rem;
    padding-right: 1rem;
}

.text-center {
    text-align: center;
}

.text-blue-900 {
    color: #1e3a8a; /* Dark blue color for headings */
}

.card {
    transition: transform 0.3s ease, box-shadow 0.3s ease; /* Smooth transition for effects */
}

.text-sm {
    font-size: 0.875rem; /* Smaller font size for text */
}

.text-gray-700 {
    color: #4b5563; /* Gray text color for better readability */
}

.leading-relaxed {
    line-height: 1.5; /* Adjusted line height for easier reading */
}

.shadow-lg {
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15); /* Shadow for the card */
}

.rounded-lg {
    border-radius: 0.5rem; /* Rounded corners for the card */
}

.hover\:scale-105:hover {
    transform: scale(1.05); /* Scale effect on hover */
}

.hover\:shadow-xl:hover {
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.25); /* Shadow effect on hover */
}

.space-y-1 > * + * {
    margin-top: 0.25rem; /* Reduced space between list items */
}

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

.py-8 {
    padding-top: 2rem;
    padding-bottom: 2rem;
}

.bg-gray-100 {
    background-color: #f7fafc; /* Light gray background for a subtle contrast */
}

.container {
    max-width: 1200px;
    margin-left: auto;
    margin-right: auto;
    padding-left: 1rem;
    padding-right: 1rem;
}

.text-center {
    text-align: center;
}

.text-blue-900 {
    color: #1e3a8a; /* Dark blue color for headings */
}

.text-4xl {
    font-size: 2.25rem; /* Size for the main heading */
}

.mb-6 {
    margin-bottom: 1.5rem; /* Margin for spacing */
}

.org-image {
    max-width: 100%; /* Responsive image */
    height: auto; /* Maintain aspect ratio */
    border: 2px solid #1e3a8a; /* Border around the image */
    border-radius: 8px; /* Rounded corners for the border */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Subtle shadow for depth */
}

.text-gray-700 {
    color: #4b5563; /* Gray text color for better readability */
}

.text-lg {
    font-size: 1.125rem; /* Size for the paragraph text */
}

.max-w-xl {
    max-width: 36rem; /* Limit the width of the paragraph */
    margin: 0 auto; /* Center the paragraph */
}

/* Upcoming event */
body {
    font-family: Arial, sans-serif; /* Default font for the body */
}

.py-8 {
    padding-top: 2rem; /* Padding for the top */
    padding-bottom: 2rem; /* Padding for the bottom */
}

.bg-gradient {
    background: linear-gradient(to right, #4a90e2, #9013fe); /* Gradient background */
    position: relative; /* Positioning context for the section */
    overflow: hidden; /* Hide overflow */
}

.container {
    max-width: 1200px; /* Max width for container */
    margin-left: auto;
    margin-right: auto;
    padding-left: 1rem; /* Padding for left */
    padding-right: 1rem; /* Padding for right */
}

.text-center {
    text-align: center; /* Center text */
}

.image-container {
    display: inline-block; /* Center the image container */
    position: relative; /* Positioning context for hover effects */
}

.org-image {
    max-width: 100%; /* Make image responsive */
    height: auto; /* Maintain aspect ratio */
    width: 450px; /* Fixed width */
    height: 300px; /* Fixed height */
    border-radius: 10px; /* Rounded corners for the image */
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3); /* Soft shadow for depth */
    transition: transform 0.3s ease, box-shadow 0.3s ease; /* Smooth transition for effects */
}

.org-image:hover {
    transform: scale(1.05); /* Slightly scale up on hover */
    box-shadow: 0 8px 40px rgba(0, 0, 0, 0.4); /* Increase shadow on hover */
}
/* Styles for the Latest News images */
.latest-news img {
    height: 200px; /* Set a fixed height */
    object-fit: cover; /* Maintain aspect ratio and cover the area */
    width: 100%; /* Ensure full width */
    border-radius: 0.5rem; /* Rounded corners for images */
}

.latest-news .news-item {
    transition: transform 0.3s; /* Smooth transition */
}

.latest-news .news-item:hover {
    transform: scale(1.05); /* Scale effect on hover */
}


.lab-item {
    transition: transform 0.3s; /* Smooth transition */
}

.lab-item:hover {
    transform: scale(1.05); /* Scale effect on hover */
}

/* Additional styles for sections */
section {
    padding: 40px 15px; /* Adding padding to sections for better spacing */
}

.footer-gradient {
    background: linear-gradient(to right, #009b4c, #f08519, #2f318b);
    color: white;
    padding: 1rem; /* p-4 */
    text-align: center; /* text-center */
}

body {
    font-family: Arial, sans-serif; /* Default font for the body */
}

.py-8 {
    padding-top: 2rem; /* Padding for the top */
    padding-bottom: 2rem; /* Padding for the bottom */
}

.bg-gradient {
    background: linear-gradient(to right, #4a90e2, #9013fe); /* Gradient background for the section */
}

.container {
    max-width: 1200px; /* Max width for container */
    margin-left: auto;
    margin-right: auto;
    padding-left: 1rem; /* Padding for left */
    padding-right: 1rem; /* Padding for right */
}

.text-center {
    text-align: center; /* Center text */
}

.event-card {
    transition: transform 0.3s ease, box-shadow 0.3s ease; /* Smooth transition for effects */
}

.event-card:hover {
    transform: translateY(-5px); /* Lift effect on hover */
}

/* Efek zoom untuk tombol */
.btn-primary {
    display: inline-block;
    background-color: #4f46e5; /* Warna biru */
    color: white;
    padding: 0.75rem 1.5rem;
    font-size: 1rem;
    font-weight: bold;
    border-radius: 0.375rem;
    transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
  }
  
  .btn-primary:hover {
    transform: scale(1.1); /* Membesarkan tombol */
    box-shadow: 0px 8px 20px rgba(0, 0, 0, 0.3); /* Menambahkan bayangan */
    background-color: #4338ca; /* Warna biru lebih gelap */
  }
  
  /* Efek zoom untuk tombol Submit */
button[type="submit"] {
  display: inline-block;
  background-color: #4f46e5; /* Warna biru */
  color: white;
  padding: 0.75rem 1.5rem;
  font-size: 1rem;
  font-weight: bold;
  border-radius: 0.375rem;
  border: none; /* Menghapus border default */
  cursor: pointer; /* Menunjukkan tombol bisa diklik */
  transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
}

button[type="submit"]:hover {
  transform: scale(1.1); /* Membesarkan tombol */
  box-shadow: 0px 8px 20px rgba(0, 0, 0, 0.3); /* Menambahkan bayangan */
  background-color: #4338ca; /* Warna biru lebih gelap */
}
