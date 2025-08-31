```sh
for file in *.{jpg,jpeg,png,bmp,tiff,tif,webp}; do
	if [[ -f "$file" ]]; then
		filename="${file%.*}";
		newfile="$filename.png";
		ffmpeg -i "$file" -y "$newfile" && rm "$file";
	fi;
done
```