# Author: xpurplexamyx
# Post URL: [https://www.reddit.com/r/Superstonk/comments/nngm4d/help_rc_is_a_master_troll_im_reasonably_sure/](https://www.reddit.com/r/Superstonk/comments/nngm4d/help_rc_is_a_master_troll_im_reasonably_sure/)


# TOP EDIT: Proven FALSE.

By replicating the technique that RC used to upload this image - creation of the tombstone in safari, followed by a long press on the picture then saving to photos and finally tweeting using the twitter for iphone app by selecting the tombstone from the photostream, I was able to exactly recreate the image that he uploaded:

    0087a321d313450fafa99dc59ad83a4c8abaf6b0  cohen_i_made_photo.jpeg
    0087a321d313450fafa99dc59ad83a4c8abaf6b0  cohen.jpeg

The cohen.jpeg is RC's version, the cohen\_i\_made\_photo.jpeg is the version that I made on my iphone, saved to my photos, and then uploaded via the twitter app. As you can see, the shasums are identical. The probability of a sha1 collision if the files were different is around 3.4\*10\^-39, and requires the generation of 10\^24 hashes to achieve. To prove that this is not a random unluckily colision, here is a sha512:

    5ba97f9e44f950c76137eb42a23eedc5c0a9f84973fad39a417319008695ed762161af629c007371f7fcb77b976caa395e159bd72fd50ddd59bbce8643697f01  cohen_i_made_photo.jpeg
    5ba97f9e44f950c76137eb42a23eedc5c0a9f84973fad39a417319008695ed762161af629c007371f7fcb77b976caa395e159bd72fd50ddd59bbce8643697f01  cohen.jpeg

Again, identical.

# This means that this post is 100% incorrect.

\---

Edit: TA;DR: [Steganography](https://en.wikipedia.org/wiki/Steganography) is the hiding of text within images and media. I think maybe Papa hid a message in the tombstone image.

A long long time ago, several past lives ago actually, this ape used to be a hacker. This was in the days of yore, when dialling into BBS's was just stopping being a thing, irc was the communications tool of choice, phone phreaking was still possible, and hacking was done predominantly to learn.

Anyway, as I sat here staring at Papa's tweet, this gnawing was going on in the back of my brain. I couldn't shake it, so I spun up a container with some useful tools and started doing some investigation on what he posted.

First of all, this is an image that I made, downloaded directly from the tombstone site:

&#x200B;

https://preview.redd.it/8qczon13zz171.jpg?width=400&format=pjpg&auto=webp&s=69e964c39437cf9e8ea7efc48bc564d5c7e2f10c

    Exif
    ====
    +---------------------+-------------------------------------------------------------+
    | key                 | value                                                       |
    +---------------------+-------------------------------------------------------------+
    | Directory           | /data                                                       |
    | Comment             | CREATOR: gd-jpeg v1.0 (using IJG JPEG v80), default quality |
    |                     |                                                             |
    | FileInodeChangeDate | 2021:05:29 04:11:52+00:00                                   |
    | ImageSize           | 400x313                                                     |
    | SourceFile          | /data/tombstone.jpeg                                        |
    | FileSize            | 35 kB                                                       |
    | JFIFVersion         | 1.01                                                        |
    | YResolution         | 180                                                         |
    | FilePermissions     | rw-r--r--                                                   |
    | FileType            | JPEG                                                        |
    | BitsPerSample       | 8                                                           |
    | Megapixels          | 0.125                                                       |
    | EncodingProcess     | Baseline DCT, Huffman coding                                |
    | ImageHeight         | 313                                                         |
    | ColorComponents     | 3                                                           |
    | FileName            | tombstone.jpeg                                              |
    | FileTypeExtension   | jpg                                                         |
    | MIMEType            | image/jpeg                                                  |
    | YCbCrSubSampling    | YCbCr4:2:0 (2 2)                                            |
    | ImageWidth          | 400                                                         |
    | XResolution         | 180                                                         |
    | FileModifyDate      | 2021:05:29 04:11:41+00:00                                   |
    | FileAccessDate      | 2021:05:29 04:44:10+00:00                                   |
    | ResolutionUnit      | inches                                                      |
    | ExifToolVersion     | 10.4                                                        |
    +---------------------+-------------------------------------------------------------+
    JPEG image data, JFIF standard 1.01, resolution (DPI), density 180x180, segment length 16, comment: "CREATOR: gd-jpeg v1.0 (using IJG JPEG v80), default quality", baseline, precision 8, 400x313, frames 3

I then tweeted it and downloaded it from there - it's not worth me adding this, the image is visually identical and I don't know what munging or compression reddit adds, so just work with me:

    Exif
    ====
    +---------------------+---------------------------------+
    | key                 | value                           |
    +---------------------+---------------------------------+
    | FileTypeExtension   | jpg                             |
    | ImageSize           | 400x313                         |
    | YCbCrSubSampling    | YCbCr4:2:0 (2 2)                |
    | ExifToolVersion     | 10.4                            |
    | FileInodeChangeDate | 2021:05:29 04:47:48+00:00       |
    | FileModifyDate      | 2021:05:29 04:13:37+00:00       |
    | JFIFVersion         | 1.01                            |
    | ResolutionUnit      | inches                          |
    | EncodingProcess     | Progressive DCT, Huffman coding |
    | FileAccessDate      | 2021:05:29 04:47:50+00:00       |
    | FilePermissions     | rw-r--r--                       |
    | Directory           | /data                           |
    | SourceFile          | /data/tombstone-twitter.jpeg    |
    | MIMEType            | image/jpeg                      |
    | FileType            | JPEG                            |
    | ImageHeight         | 313                             |
    | YResolution         | 180                             |
    | FileSize            | 32 kB                           |
    | FileName            | tombstone-twitter.jpeg          |
    | XResolution         | 180                             |
    | ImageWidth          | 400                             |
    | Megapixels          | 0.125                           |
    | BitsPerSample       | 8                               |
    | ColorComponents     | 3                               |
    +---------------------+---------------------------------+
    JPEG image data, JFIF standard 1.01, resolution (DPI), density 180x180, segment length 16, progressive, precision 8, 400x313, frames 3

As you can see from the above, twitter modifies the exif data, and removes the comment from the jpeg image data, but otherwise things remain the same.

If I run both of these images through stegdetect, I don't get anything of interest:

    root@12eac4cd5911:/data# stegdetect tombstone*
    tombstone-twitter.jpeg : negative
    tombstone.jpeg : negative

Cool. So I then remade Papa's tombstone:

&#x200B;

https://preview.redd.it/smrgyjo6zz171.jpg?width=400&format=pjpg&auto=webp&s=49e57bb246fbd58ef9c64a3ede679d913b3ced36

I repeated the same test, uploading it to twitter then downloading it again, and running it through stegdetect:

    root@12eac4cd5911:/data# stegdetect cohen_* -s 0.6
    cohen_i_made.jpg : negative
    cohen_twitter_i_made.jpeg : negative

Why did I go through all of these steps? Well, it's because if I run stegdetect on Papa's image, it finds something interesting:

    root@12eac4cd5911:/data# stegdetect cohen.jpeg -s 0.5
    cohen.jpeg : negative
    root@12eac4cd5911:/data# stegdetect cohen.jpeg -s 0.6
    cohen.jpeg : outguess(old)(*)

I'm intentionally decreasing the sensitivity here from the default of 1 to reduce the potential of a false positive. For comparison, I baked some data into my own rip dumb ass test file, to see how much would need to be added before it would detect.

    root@12eac4cd5911:/data# wc -c input
        1591 test
    root@12eac4cd5911:/data# outguess-0.13 -k "test" -d input cohen_i_made.jpg test.jpg
    root@12eac4cd5911:/data# stegdetect test.jpg -s 0.5
    test.jpg : negative
    root@12eac4cd5911:/data# stegdetect test.jpg -s 0.6
    test.jpg : outguess(old)(*)

The answer is 1591 bytes, which is equivalent to this block of random garbage latin that is completely **unrelated** other than to serve as an example of how much text 1591 bytes is:

>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum ut purus a elit dignissim condimentum vitae at ligula. Suspendisse potenti. Aliquam ultricies, sapien accumsan sodales vehicula, nibh sem pharetra ligula, non congue lorem justo feugiat augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Nam tellus est, posuere ut blandit vitae, gravida quis neque. Pellentesque vel ultricies nisi, vitae ullamcorper elit. Fusce luctus sem in eros iaculis, eu vehicula urna pulvinar. Aliquam quis pretium ipsum. Vestibulum sodales pellentesque venenatis. Proin at justo ante. Proin at nisl pellentesque, maximus arcu vel, sodales ante. Phasellus luctus turpis ligula, id gravida magna rutrum eu. Praesent malesuada tristique dui, ut egestas nibh vestibulum blandit. Curabitur pellentesque ante nulla, ac rhoncus purus malesuada a. Curabitur egestas ex non ante aliquam interdum. Fusce euismod urna in sem volutpat, id pharetra erat molestie.  
>  
>Aenean at libero mi. Ut pretium nunc eu lorem finibus sodales. Donec cursus condimentum facilisis. Maecenas tempus leo quis dignissim aliquam. Donec ornare felis sem, faucibus dapibus nisl fringilla quis. Suspendisse commodo et tellus quis pretium. Duis diam tortor, commodo condimentum massa ut, sodales viverra arcu. Aenean at lorem a tellus bibendum consequat nec et nulla. Nam nec suscipit eros. Nullam suscipit, mauris ac condimentum mollis, turpis tortor laoreet ante, fermentum dictum purus elit non lacus. Morbi laoreet aliquam dolor a consectetur. In feugiat mattis mauris a convallis. Etiam biam.

I then went ahead and extracted it and checked the shasum of the source data and extracted data:

    root@12eac4cd5911:/data# outguess-0.13 -r -k "test" test.jpg output
    root@12eac4cd5911:/data# shasum input output
    e8f1ae201384f8b025f8157eaf93e3482adcca22  input
    e8f1ae201384f8b025f8157eaf93e3482adcca22  output

Here's that image, containing the lorem text above!

&#x200B;

https://preview.redd.it/b2i7e12p00271.jpg?width=400&format=pjpg&auto=webp&s=1d04e34a6132f8505d15734ada2299fdfc85e2fd

I then uploaded my steganographic file to twitter, then downloaded it and attempted to extract the data. Whatever twitter is doing to the file bricks it:

    root@12eac4cd5911:/data# outguess-0.13 -r -k "test" E2iC6v-VkAIrsLQ.jpeg testing
    Unknown data type of E2iC6v-VkAIrsLQ.jpeg

And this is exactly the problem I'm hitting trying to get outguess-0.13 to read Papa's file. Whatever twitter's image processing is doing, is corrupting it - if there is in fact outguess steganography baked in.

    root@12eac4cd5911:/data# outguess-0.13 -r -k "stonk" cohen.jpeg papas_message
    Unknown data type of cohen.jpeg

So over to you guys... I've reached the limit of my 20+ year out of date abilities, and I'm hoping someone else who is more current with forensic steganalysis can perhaps tickle out what is baked in if there is anything.

Of course, I could be wrong, [stegdetect can throw false positives.](https://researchportal.port.ac.uk/portal/files/187568/Microsoft_Word_-_Stegdetect_article_-_Final.pdf)

Edit: Thanks to u/Lucent_Sable for kicking my brain into gear. Pulled on diffing the image data thread and what do you know:

[My version, uploaded then downloaded from twitter](https://preview.redd.it/x07m7hi680271.jpg?width=400&format=pjpg&auto=webp&s=07641d1fed66c95890ebc31633df931427bcd051)

[RC's version downloaded from twitter](https://preview.redd.it/bh38yg4980271.jpg?width=400&format=pjpg&auto=webp&s=230591f1b06390ea11dfcfcdc14ef2c86b575de4)

![Imagemagick compare diff of the images](https://preview.redd.it/k2rlpzb580271.jpg?width=400&format=pjpg&auto=webp&s=d00f9a013e13f2f51ff0d5fb711577cc681bcd91)

In terms of raw hex, there are indeed differences. A whole heap of extra data in RC's image vs mine:

    root@12eac4cd5911:/data# wc -l mytwitter.hex cohen.hex
      2134 mytwitter.hex
      2465 cohen.hex

Doing a diff of the hex data basically spits out the entire file, it is that different.

Edit: u/midgetforce2k requested pixel subtraction:

    root@12eac4cd5911:/data# convert cohen.jpeg cohen_twitter_i_made.jpeg -compose subtract -composite -threshold 0.001 -negate -alpha copy -negate mask.jpg 
    root@12eac4cd5911:/data# convert cohen.jpeg mask.jpg -composite composite.jpg 

https://preview.redd.it/vqtezlh5e0271.jpg?width=400&format=pjpg&auto=webp&s=47e7fbac70257f04913fcf0c3d5d50bf070624c1

Edit 3 May 20: Lots of requests to upload my tombstone to twitter again to see if there is any algorithmic modification taking place, or compression artifacts changing the file.

Here's the outcome of doing it through a computer, twice:

    8535a005c9d69ac348216266efb2b3d7c3710e9e  cohen_twitter_2.jpg
    8535a005c9d69ac348216266efb2b3d7c3710e9e  cohen_twitter_i_made.jpeg

As you can see, the shasum of both files, uploaded 11 hours apart then download from twitter are identical, so twitter isn't doing anything extra that would make the same image be different each time.

RC uses twitter for iphone though, so let's try that too:

    0087a321d313450fafa99dc59ad83a4c8abaf6b0  cohen_i_made_photo.jpeg
    0087a321d313450fafa99dc59ad83a4c8abaf6b0  cohen.jpeg
    234bd3c4c46137311c2c65016dcabbdd7c5ddbc5  cohen_i_made_pasted.jpeg

Well, that is simultaneously disappointing as well as revalatory.

Using the tombstone builder, then copying the outputted image and pasting it into twitter results in a different file, so we know for sure that is not the step that RC took to post this.

However, saving the tombstone to photos on the iphone and then tweeting it results in an identical shasum to the image that RC posted.

Unfortunately that means that there is definitely no steg baked into this, that this is merely a false positive caused by whatever shenanigans iOS is doing when you save an image from the web to your photos.

I feel happy but disappointed.

Final Edit: I have removed the Possible DD flair from this post and updated it to discussion as this theory has now been proven false.