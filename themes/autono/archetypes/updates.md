---
title: "{{ replace .Name "-" " " | title }}"
authors: ["Josh Ouellette"]
source_name: Name of Publication
source_url: https://www..com

## Source Thumbnail Dimensions ----------- ##
##  
##    foo.jpg         ( 500 x 330 )
##
##    ( NOTE: max-height will be 10rem (150px) on larger devices, but it will automatically center vertically and crop top and bottom using css "object-fit: cover;" )
source_thumbnail: /Autonomusings/updates/images/update-thumb.png
## --------------------------------------- ##

date: {{ .Date }}
lastmod: {{ .Date }}

## Featured Image Dimensions ----------- ##
##  
##    foo.png         ( 1500 x 1000 )
##    foo-md.png      ( 1125 x 750 )
##    foo-sm@2x.png   ( 750 x 500 )
##    foo-sm.png      ( 495 x 330 )
##
##    ( NOTE: Featured Image will only show if they go to all updates and then click on one of the updates, so this should be left with the default image almost always )
featured_image: /Autonomusings/updates/images/update
featured_type: png
## ------------------------------------- ##

categories : [ "automation" ]
tags : [ "manufacturing", "efficiency", "automation"]
layout: update
type:  "update"
highlight: false
draft: true
summarylength : 20


#######################   SHORTCODES   ########################

## Mailchimp ----------- ##
##
## {{< mailchimp >}}
##
## --------------------- ##  ( NOTE: You can change list/subscription configuration in /data/mailchimp.toml )

## Image --------------- ##
##
## {{< img src="/interviews/jack-ryan/interview" type="png" alt="" caption="On site at Renham Industries" >}}
##
## --------------------- ##  ( NOTE: allows for responsive suffixes to be added automatically -- caption preferable but not necessary )

## Soundcloud ---------- ##
##
## {{< soundcloud 412671942 >}}
##
## --------------------- ##  ( NOTE: You can change list or account configuration in /data/mailchimp.toml )



#######################   FORMATTING   ########################

## Pullqoute ----------- ##
##
## {{% pullquote left %}} "Sollicitudin ornare odio blandit" {{% /pullquote %}} 
##
## --------------------- ##  ( NOTE: left is preferable, but you can do right if you'd like )

## Blockquote ---------- ##
##
## >Sollicitudin . . .
##
## --------------------- ##  ( NOTE: blockquotes with multiple lines or lists or bullets require ">" for each line )

---

### What Happened:
At quisque litora ullamcorper maecenas ultricies ut dignissim luctus curabitur, cras congue eget primis aliquam fringilla nulla dictum posuere, vestibulum sit magnis nisl praesent eros ipsum nunc.

### Why It Matters:
At quisque litora ullamcorper maecenas ultricies ut dignissim luctus curabitur, cras congue eget primis aliquam fringilla nulla dictum posuere, vestibulum sit magnis nisl praesent eros ipsum nunc.
