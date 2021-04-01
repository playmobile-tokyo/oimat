# url
https://www.tensorflow.org/tutorials/images/classification?hl=ja

# rename
rename -v 's/\.(jpeg|JPG|JPEG)/\.jpg/' *
rename 's/.jpeg/.jpg/' *.jpeg
ls *.jpg | awk '{ printf "mv %s %03d.jpg\n", $0, NR }' | sh

#
