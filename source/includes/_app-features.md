#App Features

## Earlham Day


Earlham Day is a single day that Earlham seeks donations, to help continue the goals of Earlham. In prior years updates on the day had to manually be edited. Starting in 2017 donation data is updated in close to real-time.


## Earlham Day - Goal (Macro)

```json
    "goalfolder":{
      "Alias": "goalfolder",
      "Name": "Goal Folder",
      "Type": "Content Picker"
    }
```
<aside class="notice">AJAX Automatically loads new data without page refresh</aside>
### Site Wide Goals
### Donation Goals
## Earlham Day - Recent Donations (Macro)
```json
    "donationCount":{
      "Alias": "donationCount",
      "Name": "Max # of Donations",
      "Type": "Number"
    }
```
<aside class="notice">AJAX Automatically loads new data without page refresh</aside>
<img src='/images/apps/earlhamday/recent-donations.png'/>

## Podcasts [Macro]

<aside class="notice">The macro takes a soundcloud username ex:earlhamcollege</aside>


### Main Podcasts Home page

Dependency | Description | Link to Doc
-------------- | -------------- | --------------
Readmore.js | To collapse long descriptions of podcasts to a specific height. | http://jedfoster.com/Readmore.js/

**Image**
<img src='/images/apps/podcasts/podcast-home-page.png'/>


### Individual Podcasts pages

Dependency | Description | Link to Doc
-------------- | -------------- | --------------
Clipboard.js | To copy link of podcast to clipboard. | https://clipboardjs.com/

**Image**
<img src='/images/apps/podcasts/podcast-individual-page.png'/>

## Tiles

### Course tiles

```html
@using umbraco.MacroEngines
@using umbraco.MacroEngines.Library
@inherits umbraco.MacroEngines.DynamicNodeContext
<!-- Isotope Filters
=================================== -->
<div class="isotope-filters">
<div class="filter option-set" data-filter-group="programs">
<!-- Button Row -->
<div class="row">
<div class="col-sm-12">
<a class="btn btn-isotope" data-filter-value=".natural-sciences" href="#division-natural-sciences-division"><i class="icon-check-empty"></i> Natural Sciences</a>
<a class="btn btn-isotope" data-filter-value=".social-sciences" href="#division-social-sciences-division"><i class="icon-check-empty"></i> Social Sciences</a>
<a class="btn btn-isotope" data-filter-value=".humanities" href="#division-humanities-division"><i class="icon-check-empty"></i> Humanities</a>
<a class="btn btn-isotope" data-filter-value=".global-and-cultural" href="#division-global-and-cultural"><i class="icon-check-empty"></i> Global/Cultural</a>
<a class="btn btn-isotope" data-filter-value=".visual-and-performing-arts" href="#division-visual-proforming-arts"><i class="icon-check-empty"></i> Visual/Performing Arts</a>
<a class="btn btn-isotope btn-isotope-refresh" href="javascript:void(0);"><i class="icon-refresh"></i> Refresh<a>
</div><!-- /.col -->
</div><!-- /.row -->
</div><!-- /.option-set -->                                     
</div><!-- /.isotope-filters -->
```

<aside class="notice">To Edit in Umbraco:</aside>
The data placeholder is under Content > Institution > Degree Programs. 

The main application file is under Developer > Scripting Files > application-degree-programs.cshtml

<img src='/images/apps/tiles/department_tiles.PNG'/>


### Profile/Story tiles
<aside class="notice">To Edit in Umbraco:</aside>

The macro is under **Developer > Scripting Files**. The file names start with **app-profile**.

The content is under **Content > Features** and each of those files have associations to other relevant pages.

<img src='/images/apps/tiles/stories.PNG'/>

