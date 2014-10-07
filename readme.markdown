jQuery File Validation
======================

Uploading files, only to find that they are too large, or the wrong type is frustrating.
The `fileValidator` plugin lets you warn users before they start uploading 
enormous files.
<p>This is forked from <a href="https://github.com/adamsanderson">adamsanderson's</a> <a href="https://github.com/adamsanderson/jQuery-File-Validator">jQuery-File-Validator</a>
Usage
-----
Simply select the file inputs you wish to validate, and pass in a callbacks to handle invalid files.

	$( el ).fileValidator({
		onValidation: function(files){ /* Called once before validating files */ },
		onInvalid:    function(validationType, file){ /* Called once for each invalid file */ },
		onValid:    function(file){ /* Called once for each valid file */ },
		maxSize:      '2m', //optional
		type:         'image' //optional
	});