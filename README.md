# :boom: re-cover | Hugo theme for recovery groups

Live Demo: **[here](https://re-cover-hugo-demo.netlify.app/)**

![re-cover cover image](https://github.com/sieis/re-cover/blob/main/static/images/recover-theme.jpg?raw=true)

This is meant to address the more common web needs of a group. Namely, a clean, readable and easily accessible site for any member to:

1. Find basic information about the meeting. i.e. location, times, format.
1. Access the meeting guide and participate without the need for paper handouts.
1. Access any online only meeting resources.
1. Contribute donations to the group easily online.

![template screenshot](https://raw.githubusercontent.com/sieis/re-cover/main/images/screenshot.png)

## Installation & Usage

1. Make a new hugo site and clone theme into theme folder:

```
$ hugo new site yoursitename
$ cd yoursitename
$ git clone git@github.com:sieis/re-cover.git themes/recover
```

2. Copy contents of /themes/exampleSite into ```yoursitename``` root directory.

```
 $ hugo server -D
```

## 12 Step Groups

The example site included in the template is based upon The Beagle Pack's web page project, and the inception of this theme was brought about after having built similar sites for different groups.

For much of the configuration, editing the config.toml file will suffice. Particularly for groups with limited customization needs, this will provide plenty of the basic needs for a group or meeting's home page.

**This project was built out of a need for a simple, fast, easily accessible and modern web site to host an AA group's readings and donation information.**

In many cases, the site may be hosted for free with the only optional expense being a yearly domain registration if custom domain names are required. (i.e. meetingname.com or meetingname.org)


## Area Intergroups

Local Intergroups may also find this theme useful. Please contact me if your needs stretch beyond the simplicity of this theme. 

I have worked with intergroups to provide custom solutions to existing sites.


## CONFIG

Much of the data specific to each group is contained within the config.toml file. Copy and modify this from the exampleSite in order to change the specifics listed on almost every section of the template.

## Colors

The theme is provided with custom coloring and pictures which match. The main.css file may be modifed to add or remove any of these choices, and you may replace the images with new ones of your own choosing as well. There are many available resources for images. One such is [unDraw](https://undraw.co/) which I've utlized for the stock images in this theme.

## Icons

I've used [Font Awesome](https://fontawesome.com/), albeit sparingly, and have it loading via CDN. 

## Meta Data

In the head partial, several pieces of meta data are set for the title, description, og:image and favicon. Edit these as you see fit. Favicons are stored in /static/favicons/.

## Regular Readings

Many popular readings are included under the Regular Readings section. These may be changed if desired. The readings are in the content -> readings folder as individual markdown files. Setting the draft to true will deactivate any of these. 

You may add additional readings by creating new markdown files in the readings folder.

## Readings List

There is a Readings List page (/readings/) that is not actively linked, but which can be if needed. It simply holds a list of each of the available readings that are available in the modal drop-down menus on the home page. The template controling this is the section.html in the default layouts folder. Likewise, there is a single.html template which controls the individual readings pages.

## About the meeting

For meeting and/or chairperson guidelines specific to your group, the about page includes placeholder elements. In the example, chairperson guidelines are listed in six sections. These may be edited, removed, or added to via the data folder. The guidelines in use are contained within the guidelines.json file in the data folder.

## Blog, or a lack thereof

The base template does not have proper blog functionality, though it could be added if a group needed it. 
