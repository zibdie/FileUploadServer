# File Transfer Server

A simple Node.js server that allows users to transfer files of any size. Files are stored in the `uploads` directory. You can run this locally by spinning up the the server and then using [ngrok](https://ngrok.com/) to get a public URL. **This is not a file hosting service, this is for transferring files from one PC to another when its difficult to use remote software**

**Use Case:** If you need to transfer files from another PC you dont trust and do not want to login in from. Also, sometimes you may only get access to the server with the Virtualbox/Hyper-V window itself and cannot RDP.

## Features

- No file size limits
- Drag and drop support
- Modern UI
- Simple and easy to use

## Setup

1. Install dependencies:
```bash
npm install
```

2. Start the server:
```bash
npm start
```

3. Open your browser and navigate locally to give it a test:
```
http://localhost:3000
```

## Usage

1. Click the upload area or drag and drop a file
2. Click the "Upload File" button
3. Wait for the upload to complete
4. Files will be stored in the `uploads` directory with a timestamp prefix
5. (Optional) Run `ngrok http 3000` to get a URL.

## Technical Details

- Built with Express.js
- Uses Multer for file upload handling
- Files are stored with timestamp prefixes to prevent naming conflicts
- No file size restrictions 