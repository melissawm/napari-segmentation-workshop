# Installing napari plugins

#### Pre-Requisites
Successful installation of napari (see [napari installation tutorial](https://chanzuckerberg.github.io/napari-segmentation-workshop/onboard/gettingstarted.html)).

## Overview of the napari hub

<script src="https://fast.wistia.com/embed/medias/md1jundqsq.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:64.79% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_md1jundqsq seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/md1jundqsq/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

The reader is highly encouraged to visit the napari hub prior to installation of plugins to browse available plugins, read descriptions, review documentation, and see links to developer content.  Taking a few minutes to review options to ensure a plugin is right for your intended application  in this way can be invaluable in saving time later on. For example, some plugins have specific recommendations for how to install, which may be different from the steps outlined below.

## Plugin Installation Tutorial

<script src="https://fast.wistia.com/embed/medias/em0g2n34k7.jsonp" async></script><script src="https://fast.wistia.com/assets/external/E-v1.js" async></script><div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><div class="wistia_embed wistia_async_em0g2n34k7 seo=false videoFoam=true" style="height:100%;position:relative;width:100%"><div class="wistia_swatch" style="height:100%;left:0;opacity:0;overflow:hidden;position:absolute;top:0;transition:opacity 200ms;width:100%;"><img src="https://fast.wistia.com/embed/medias/em0g2n34k7/swatch" style="filter:blur(5px);height:100%;object-fit:contain;width:100%;" alt="" aria-hidden="true" onload="this.parentNode.style.opacity=1;" /></div></div></div></div>

## Introduction
A user may ask why programs such as napari require plugins to accomplish certain functions, or add additional functionality.  There are many reasons behind this, but two of the most common ones are:

- By providing a core viewer without plugins pre-installed, it enables the program to enjoy a so-called “light weight” installation, which minimizes the burden on user machines.  This makes sense when one considers the myriad plugins available over time, a researcher’s need to perhaps on need a few, and the widely varying performance capabilities of user computers.

- Plugins are dependent on associated files that come along with their installation (i.e.: a particular library). Several plugins may share such dependencies. However, it is not uncommon for the version of these dependencies to be different. For example, Plugin A may require the newest version of a particular library to be functional, whereby Plugin B may not be compatible with the latest version. This can be frustrating for users when too many plugins (and thus too many dependencies) are having to be managed. By keeping installed plugins to only those required for a particular users work, it can minimize such issues.

This is also a good time to remind the reader of why virtual environments can be especially helpful. Not only do they keep particular installations contained, one can also create (or delete) many virtual environments, with different installations of plugins, etc… for specific types of analyses.

Installation of plugins into napari is usually a very straightforward process. Please note that there is more than one way to install a plugin (GUI vs. command line, for example). We’ll cover the basics of the GUI-based installation, such that prior coding knowledge is not required.

:::{hint} Note: It is always good to remember that with any open-source program with a constantly evolving repository of plugins, the relative “maturity” of a plugin can widely vary. For example, some plugins may be intuitive to install, use, and are well-documented, vs. others that are not.
:::


