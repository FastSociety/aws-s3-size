# AWS S3 Folder Size Calculator
This module does one thing. It will calculate the total size of a folder inside of S3.

Installation

    npm install aws-s3-size

Example Usage

    var S3Sizer = require('aws-s3-size');
    configFile = __dirname + '/awscreds.json',
    s3Sizer = new S3Sizer({configFile : configFile});

    s3Sizer.getFolderSize('bucket.name', 'foldername', function(err, size) {
      console.log(size)
    });