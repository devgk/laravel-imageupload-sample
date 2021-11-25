1. $request->hasFile('photo'); (To check the request key is a valid file)

2. movie.mp4 / images.jpg / .png / .gif / document.doc / sheets.xls / datasheet.csv	
		$extension = $request->photo->extension();
		
3. $name = 'my-image.'.$extension;

4. $request->image->storeAs(
        '',         	// Folder
        $name,     					// Name
        'public'					// public
    );
	
5. Use this in form where we upload image (enctype="multipart/form-data")


To install bootstrap with user authentication template
php artisan ui bootstrap --auth