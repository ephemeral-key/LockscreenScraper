#!/usr/bin/env python
#Author: https://github.com/ephemeral-key/
#Python script to pull Windows 10 Lockscreen Images to a new desktop folder (lockscreen_images) and convert them to JPEGs

import shutil, os, sys, time

src = os.path.expanduser("~/AppData/Local/Packages/Microsoft.Windows.ContentDeliveryManager_cw5n1h2txyewy/LocalState/Assets")
target = os.path.expanduser("~/Desktop/lockscreen_images")

shutil.copytree(src, target)

folder = target
for filename in os.listdir(folder):
       infilename = os.path.join(folder,filename)
       if not os.path.isfile(infilename): continue
       oldbase = os.path.splitext(filename)
       output = os.rename(infilename, infilename + '.jpg')

def printart():
    print """
                    
                   .               ,.
                  T."-._..---.._,-"/|
                  l|"-.  _.v._   (" |
                  [l /.'_ \; _~"-.`-t
                  Y " _(o} _{o)._ ^.|   Success!
                  j  T  ,-<v>-.  T  ]
                  \  l ( /-^-\ ) !  !
                   \. \.  "~"  ./  /c
                     ^r- .._ .- .-" 
                     """


printart()      
print 'Images are located at ' + target
