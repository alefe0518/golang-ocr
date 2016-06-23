# go-tesseract-ocr-service

This Golang based project provides a microservice that offers a REST API and a Web
view to convert PDF's and Images to Text.

Just a proof-of-concept at this point. For future development it will be split in a
multi-tier application architecture for better escalability - again for instructional
purposes.

####All you need to do is clone this repo:

```
docker-compose up --build
```

####Main webviews
```
http://localhost:8080/view
http://localhost:8080/web/pdf
http://localhost:8080/web/img
```

####API Endpoints for PDF submission
```
http://localhost:8080/api/upload/pdf
```
####API endpoint for Image submission
```
http://localhost:8080/api/upload/img
```

####Frameworks
This projects uses the following SDK's:
- [Tesseract OCR](http://github.com/tesseract-ocr) : OCR Engine
- [GhostScript](http://www.ghostscript.com): PDF interpreter used to convert PDF to a set of images (per page)

(C)June 2016
