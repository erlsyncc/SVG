# SVG Converter Web App

A simple web application that converts uploaded images into SVG (Scalable Vector Graphics) using the SVG.new API.

## Project Description

This project demonstrates how to integrate a public API into a web application. Users can upload an image, which is sent to the SVG.new API for processing. The generated SVG is then displayed on the website and can be downloaded.

## Features

- Upload PNG, JPG, or JPEG images
- Convert images to SVG using the SVG.new API
- Display the generated SVG
- Download the converted SVG
- Error handling for invalid uploads and API failures

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Axios (or Fetch API)
- SVG.new API

## Project Structure

```
project/
│
├── public/
│   ├── css/
│   ├── js/
│   └── uploads/
│
├── views/
│   ├── index.html
│   └── result.html
│
├── routes/
│   └── api.js
│
├── app.js
├── package.json
├── .env
└── README.md
```

## Installation

1. Clone the repository.

```bash
git clone https://github.com/yourusername/svg-converter.git
```

2. Navigate to the project folder.

```bash
cd svg-converter
```

3. Install dependencies.

```bash
npm install
```

4. Create a `.env` file.

```env
API_KEY=YOUR_SVG_NEW_API_KEY
```

5. Start the application.

```bash
npm start
```

or

```bash
node app.js
```

6. Open your browser.

```
http://localhost:3000
```

## How It Works

1. The user uploads an image.
2. The server sends the image to the SVG.new API.
3. The API processes the image and generates an SVG.
4. The application displays the SVG.
5. The user can download the generated SVG.

## API Used

SVG.new API

Documentation:
https://svg.new/

## Error Handling

The application handles:

- Invalid file uploads
- Missing image files
- API request failures
- Network connection errors
- Server errors

## Future Improvements

- Drag and drop image upload
- Image preview before conversion
- Conversion history
- User authentication
- Dark mode

## Author/s

- Combenido, Earlsin Mae G.
- Consigo, Rica Mae G.
- Tariao, Bernadette B.

## License

This project is created for educational purposes.
