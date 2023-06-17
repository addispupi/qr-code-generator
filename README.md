# QRCode Generator
A simple QR Code generator using official qrcode.min javascript.

## Usages
```
document.getElementById("qr-btn").addEventListener("click", function(e) {
    // Initialize & Get references to elements
    var value = document.getElementById("qr-input").value; // Get QR Value
    var box = document.querySelector(".qr-box"); // Get QR Container

    // Test entered values
    console.log(value);

  if (value !== null) {
    // Generate QR code using the entered value
    const qrCode = new QRCode(box, { text: value,
      width: 200,
      height: 200,
      colorDark: "#000000",
      colorLight: "#FFFFFF"
    });
  }
});
```
### SAMPLE SCREENSHOT
![UI QRCode Generator Image](https://github.com/addispupi/qr-code-generator/blob/main/assets/img/ss_qr_ui.png)
