// Resimlerin bulunduğu dizin
const imageDirectory = "images/";

// Resimlerin adları
const avengersImages = [
    "ironman basketbolcu.jpeg",
    "Captan America.jpeg",
    "Thor basketbolcu.jpeg",
    "hulk basketbolcu.jpeg",
    "blackwidow basketbolcu.jpeg",
    "hawkeye basketbolcu.jpeg",
    "Spiderman basketbolcu.jpeg",
    "Blackpanther basketbolcu.jpeg"
];

// Galeri alanını seç
const gallery = document.querySelector(".gallery");

// Her bir resim için bir img elementi oluştur ve galeriye ekle
avengersImages.forEach(imageName => {
    const img = document.createElement("img");
    img.src = imageDirectory + imageName;
    img.alt = imageName.split(".")[0]; // Dosya uzantısını kaldırarak resim ismini al
    gallery.appendChild(img);
});
