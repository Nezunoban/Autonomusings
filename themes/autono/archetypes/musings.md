---
title: "{{ replace .Name "-" " " | title }}"
authors: ["Josh Ouellette"]
date: {{ .Date }}
lastmod: {{ .Date }}

## Featured Image Dimensions ----------- ##
##  
##    foo.png         ( 1500 x 1000 )
##    foo-md.png      ( 1125 x 750 )
##    foo-sm@2x.png   ( 750 x 500 )
##    foo-sm.png      ( 495 x 330 )
##
featured_image: /Autonomusings/musings/images/musing
featured_type: png
## ------------------------------------- ##

## Categories: ( NOTE: Every Musing needs 1 category )
categories : [ "automation" ]

tags : [ "manufacturing", "efficiency", "automation"]
layout: musing
type:  "musing"
highlight: false
draft: true
summarylength : 20

## Do you want the executive summary for this post?
executive_summary: true

## A sentence or two to summarize the piece ('' required for colon)
executive_intro : 'In this musing, we discuss the matter at hand, including:'

## Bullet Point Summary - Up to 5 points allowed 
executive_point1 : The matter at hand
executive_point2 : Of course we also touch on the importance of the matter at hand, for educational purposes, including long points
executive_point3 : The matter at hand


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

**Insert Lead paragraph here.**

A augue nunc lacus auctor efficitur tempor placerat, dictum volutpat mi vitae viverra porta non sem, himenaeos senectus vivamus potenti cubilia sollicitudin. Curae cursus inceptos tincidunt magna mi nibh ad enim etiam, molestie eu quis primis hendrerit taciti phasellus. Feugiat ultricies dictumst iaculis potenti odio laoreet urna at, ultrices curae leo accumsan proin sem lobortis.

## Heading 2

Sollicitudin ornare odio blandit aenean enim lacus accumsan elementum vestibulum porta mauris lorem, ullamcorper class fermentum sem hendrerit ante augue penatibus scelerisque felis leo proin,ad nascetur venenatis sodales dignissim viverra suspendisse turpis convallis condimentum sapien.

### Heading 3

At quisque litora ullamcorper maecenas ultricies ut dignissim luctus curabitur, cras congue eget primis aliquam fringilla nulla dictum posuere, vestibulum sit magnis nisl praesent eros ipsum nunc. Ligula lacus ipsum orci aenean integer pharetra habitasse interdum, porttitor etiam hac feugiat placerat morbi posuere turpis leo, quam at amet gravida commodo fringilla erat.
