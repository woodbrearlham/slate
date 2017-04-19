# Navigation

## Main navigation

```csharp
@using umbraco.MacroEngines;
@using umbraco.NodeFactory;
<a class="hide-accessible" href="#body" id="skip-to-content">Skip to Content</a>
<div class="ec-sites-navigation">
<div ontouchstart="return true;" class="video-modal-opened video-modal-close-trigger video-modal-toggle" id="video-modal">
<button ontouchstart="return true;" type="button" class="video-modal-close-trigger" id="video-modal-close" data-dismiss="modal">Close</button>
<div class="container">
<div class="row">
<div class="col-md-10 col-md-offset-1">
<div class="embed-responsive embed-responsive-16by9">
<iframe class="embed-responsive-item"></iframe>
</div>
</div>
</div>
</div>
</div><!-- .video-modal-open -->
<div class="mobile-navigation flyout" id="mobileNav">
<a style="cursor:pointer;" id="mob-menu-close-btn" class="btn-flyout-close">
<span class="l"></span>
<span class="l"></span>
<span class="l"></span>
</a>
<ul id="#mainNav">
<li class="@GetActiveClass("About")">
<a href="/about/">About</a>
</li>
<li class="@GetActiveClass("Academics")">
<a href="/academics/">Academics</a>
</li>
<li class="@GetActiveClass("Student Life")">
<a href="/student-life/">Student Life</a>
</li>
<li class="@GetActiveClass("Admissions")">
<a href="/admissions/">Admissions</a>
</li>
<li class="@GetActiveClass("Athletics")">
<a href="http://www.goearlham.com/">Athletics</a>
</li>
<li class="@GetActiveClass("Outcomes")">
<a href="/outcomes/">Outcomes</a>
</li>
</ul>
<ul id="#auxNav">
<li class="@GetActiveClass("Epic")">
	<a href="/epic/" style="text-transform:capitalize; font-style: italic; padding: 10px; background-color: darkgray;"><i class="fa fa-info-circle"></i> The EPIC Advantage</a>
</li>
<li>
<a href="/parents/"><i class="fa fa-user"></i>Parents</a>
</li>
<li>
<a href="/alumni/"><i class="fa fa-globe"></i>Alumni</a>
</li>
<li>
<a href="/giving/"><i class="fa fa-gift"></i>Giving</a>
</li>
<li>
<a href="javascript:void(0)"><i class="fa fa-lock"></i>The Heart</a>
</li>
</ul>
</div>
<div class="flyout-navigation flyout" id="flyoutNav">
<!--<a href="#" id="flyout-menu-close-btn" class="btn-flyout-close">
<i class="fa fa-times"></i>
</a>-->
<ul id="prospective-students-links">
<li><h4>Prospective Students</h4></li>
<li><a href="https://explore.earlham.edu/Datatel.ERecruiting.Web.External/Pages/prospectinquiry.aspx?f=90a1f936-1567-42e7-a371-0ce961acb10e">Request Information</a></li>
<li><a href="http://earlham.edu/admissions/apply/">How to Apply</a></li>
<li><a href="https://explore.earlham.edu/Datatel.ERecruiting.Web.External/Pages/welcome.aspx">Sign Up With Explore Earlham</a></li>
<li><a href="http://earlham.edu/academics/">Find My Major</a></li>
<li><a href="http://earlham.edu/admissions/visit/">Visit Our Campus</a></li>
<li><a href="http://earlham.edu/admissions/contact-us/">Connect With an Admissions Counselor</a></li>
<li><a href="http://earlham.edu/admissions/international-admissions/">For International Students</a></li>
<li><a href="/epic">Learn about the EPIC Advantage</a></li>
</ul>
<ul id="current-students-links">
<li><h4>Current Students</h4></li>
<li><a href="http://earlham.edu/academics/academic-calendar/">Academic Calendar</a></li>
<li><a href="http://earlham.edu/curriculum-guide/">Curriculum Guide</a></li>
<li><a href="http://earlham.edu/student-life/student-activities/student-organizations/">Student Organizations</a></li>
<li><a href="http://earlham.edu/student-life/student-leadership/student-government/">Student Government</a></li>
<li><a href="http://earlham.edu/academics/off-campus-study/">Off-Campus Study</a></li>
<li><a href="http://earlham.edu/center-for-integrated-learning/">Center for Integrated Learning</a></li>
<li><a href="https://tentram.earlham.edu:8250/pls/frog/bwckschd.p_disp_dyn_sched">Class Schedules</a></li>
</ul>
</div>
<div class="search-bar search-closed" id="search">
<div class="container">
<div class="row">
<form class="input-group" action="//www.earlham.edu/search/" method="get">
<input name="q" type="text" id="search_input" class="form-control" placeholder="Search Earlham..." title="Press Enter to begin search..." autofocus="">
<a style="cursor:pointer;" class="search-button search-toggle"><i class="fa fa-remove"></i></a>
</form>
</div><!-- /.row -->
</div><!-- /.container -->
</div><!-- /.search-bar -->
<nav class="aux-navigation">
<div class="container-fluid" >
<div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
<ul class="nav navbar-nav">
<li class="modal-btn"><a href="http://earlham.edu/ctcl/" style="padding-top: 0; padding-bottom: 0;">Earlham is among the select <span style="font-style: italic;">Colleges That Change Lives.</span> Learn More <i class="fa fa-chevron-right"></i></a></li>
</ul>
<ul class="nav navbar-nav navbar-right" id="auxNav">
<li>
<i class="fa fa-user"></i>
<a href="/parents/">Parents</a>
<ul class="tooltip-menu" id="#tooltip-parents">
<li><a href="/parents/how-do-i/">How do I ...</a></li>
<li><a href="/parents/academic-advising-information-from-the-registrars-office/">Academic Advising</a></li>
<li><a href="https://earlham.afford.com/">Student Account Center</a></li>
<li><a href="/maps/">Maps &amp; Directions</a></li>
</ul>
</li>
<li>
<i class="fa fa-globe"></i>
<a href="/alumni/">Alumni</a>
<ul class="tooltip-menu" id="#tooltip-alumni">
<li><a href="https://www.earlham.edu/classnotes/">Class Notes</a></li>
<li><a href="/alumnievents/">Alumni Events</a></li>
<li><a href="/homecoming/">Homecoming &amp; Reunions</a></li>
<li><a href="/update-info/">Update Your Info</a></li>
</ul>
</li>
<li>
<i class="fa fa-gift"></i>
<a href="/giving/">Giving</a>
<ul class="tooltip-menu" id="#tooltip-donors">
<li><a href="/online-giving/">Make a Gift</a></li>
<li><a href="/giving/funding-priorities/">Funding Priorities</a></li>
<li><a href="http://earlham.myplannedgift.org/">Planned Giving</a></li>
<li><a href="/giving/giving-stories/">Giving Stories</a></li>
</ul>
</li>
<li>
<i class="fa fa-lock"></i>
<a href="https://theheart.earlham.edu">The Heart</a>
<ul class="tooltip-menu" id="#tooltip-theheart">
<li><a href="https://theheart.earlham.edu">Portal (theHeart)</a></li>
<li><a href="https://earlham.advisestream.com">AdviseStream</a></li>
<li><a href="https://moodle.earlham.edu/">Moodle</a></li>
<li><a href="https://epress.earlham.edu/">ePress</a></li>
<li><a href="https://www.earlham.edu/mail/">Email</a></li>
<li><a href="http://library.earlham.edu/">Library</a></li>
<li><a href="https://25live.collegenet.com/earlham/">Events (25Live)</a></li>
<li><a href="/the-heart/">Intranet</a></li>
</ul>
</li>
<li><i class="fa fa-search"></i><a class="search-toggle" style="cursor:pointer;">Search</a></li>
</ul>
</div><!-- /.navbar-collapse -->
</div><!-- /.container-fluid -->
<div class="flyout-menu">
<a class="open-menu" id="flyout-menu-toggle">
<span class="l"></span>
<span class="l"></span>
<span class="l"></span>
</a>
</div>
</nav>
<nav class="main-navigation">
<div class="container-fluid" style="max-width:1140px;margin: 0 auto;">
<div class="navbar-header">
<a class="navbar-brand" href="/">
<img class="site-logo" alt="Earlham College Logo" src="//earlham.edu/img/earlham-college.png">
</a>
</div>
<a style="cursor:pointer;" id="mob-menu-toggle">
<i class="fa fa-bars"></i>
<span>Menu</span>
</a>
<a style="cursor:pointer;" class="search-toggle" id="mob-search-toggle">
<i class="fa fa-search"></i>
<span>Search</span>
</a>
<div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
<ul class="nav nav-justified" id="mainNav">
<li class="@GetActiveClass("About")">
<a href="/about/">About</a>
</li>
<li class="@GetActiveClass("Academics")">
<a href="/academics/">Academics</a>
</li>
<li class="@GetActiveClass("Student Life")">
<a href="/student-life/">Student Life</a>
</li>
<li class="@GetActiveClass("Admissions")">
<a href="/admissions/">Admissions</a>
</li>
<li class="@GetActiveClass("Athletics")">
<a href="http://www.goearlham.com/">Athletics</a>
</li>
<li class="@GetActiveClass("Outcomes")">
<a href="/outcomes/">Outcomes</a>
</li>
</ul>
</div><!-- /.navbar-collapse -->
</div><!-- /.container-fluid -->
</nav>
</div>
<script>
  $(document).ready(function(){
	$('#prospective-students-links a[href="/epic"]').on('click', function(e){
		ga('send', 'event', 'navigation-click', 'nav-click', 'Desktop side-nav Learn About the EPIC Advantage');
	});

	  $('.mobile-navigation a[href="/epic/"]').on('click', function(e){
		ga('send', 'event', 'navigation-click', 'nav-click', 'Mobile side-nav The EPIC Advantage');
	});
	  $('.aux-navigation a[href="http://earlham.edu/ctcl/"]').on('click', function(e){
		  ga('send', 'event', 'navigation-click', 'nav-click', 'Header: Colleges That Change Lives');
	});
  });
</script>
@functions {
public int id {get; set;}
public int startId {get; set;}
public DynamicNode currentNode {get; set;}
public DynamicNode previousNode {get; set;}
public DynamicNode deptNode {get; set;}
public DynamicNode sectionNode {get; set;}
protected override void InitializePage()
{
base.InitializePage();
int currentNodeId = 0;
if (!int.TryParse(Request.QueryString["id"], out currentNodeId))
{
currentNodeId = Model.Id;
}
currentNode = Model.NodeById(currentNodeId);
deptNode = currentNode.AncestorOrSelf("DeptHome");
if (currentNode.AncestorOrSelf("Home") != null)
{
// We are under "Home"
sectionNode = currentNode.AncestorOrSelf("SectionPage");
}
else if (deptNode != null)
{
// We are under "Academic Departments" or "Department"
int startNode = int.Parse(deptNode.GetProperty("startNode").Value);
sectionNode = Model.NodeById(startNode).AncestorOrSelf("SectionPage");
}
else
{
// We are some other kind of page, like a "Profile"
int previousNodeId = 0;
int.TryParse(Request.QueryString["r"], out previousNodeId);
if (previousNodeId > 0)
{
previousNode = Model.NodeById(previousNodeId);
deptNode = previousNode.AncestorOrSelf("DeptHome");
if (deptNode != null)
{
int startNode = int.Parse(deptNode.GetProperty("startNode").Value);
sectionNode = Model.NodeById(startNode).AncestorOrSelf("SectionPage");
}
else
{
sectionNode = previousNode.AncestorOrSelf("SectionPage");
}
}
}
}
public IHtmlString GetSectionName()
{
return Html.Raw(sectionNode.GetProperty("title").Value);
}
public string GetActiveClass(string sectionName)
{
if (sectionNode == null) return "";
return sectionNode.Name == sectionName ? "active" : "";
}
}

```

<img src='/images/navigation/main_nav.png'/>

## Slide-in navigation

<img src='/images/navigation/slide_in.png'/>

## Side navigation

```csharp

// navigation-navbar-links.cshtml

@using umbraco.MacroEngines
@using umbraco.MacroEngines.Library
@inherits umbraco.MacroEngines.DynamicNodeContext
@{                  
int toNode = @Model.Id;
if (!int.TryParse(Request.QueryString["r"], out toNode))
{toNode = @Model.Id;}
}

@helper traverse( dynamic node, dynamic refNode )
{
  bool active = Array.IndexOf(@refNode.Path.Split(','), @node.Id.ToString()) >= 0 ? true : false;
  string activeClass = @active ? "class=active" : "";
	string url = "";
	string target = "";
	if (@node.NodeTypeAlias == "Link"){
	url= (@node.HasValue("linkInternal") ? @Model.NodeById(@node.linkInternal).Url : @node.linkExternal);
		target = (@node.linkNewWindow ? " target=\"_blank\"" : "");}
	else{
	url = @node.Url;	
	}

 
 if( @node.Level == 2 )
 {
 
 <ul class="nav nav-level1">
	 @foreach( var child in @node.Children.Where("Visible").Where("NodeTypeAlias != @0", "Tab") )
    {
      @traverse( @child, @refNode );                            
    }
  </ul>
 } else if ( @node.Level == 3 )
 {
    <li @activeClass><a href="@url"@target>@( @node.menuLabel != "" ? @node.menuLabel : @node.Name )</a>
      @if ((@active == true) && (@node.Children.Where("Visible").Where("NodeTypeAlias != @0", "Tab").Count() > 0))
      {
        <ul class="nav nav-level2">
          @foreach( var child in @node.Children.Where("Visible").Where("NodeTypeAlias != @0", "Tab") )
          {
            @traverse( @child, @refNode );                            
          }
        </ul>
      }
    </li>
 } else if ( @node.Level == 4 )
 {
    <li @activeClass><a href="@url"@target>@( @node.menuLabel != "" ? @node.menuLabel : @node.Name )</a>
      @if ((@active == true) && (@node.Children.Where("Visible").Where("NodeTypeAlias != @0", "Tab").Count() > 0))
      {
        <ul class="nav nav-level3">
          @foreach( var child in @node.Children.Where("Visible").Where("NodeTypeAlias != @0", "Tab") )
          {
            @traverse( @child, @refNode );                            
          }
        </ul>
      }
    </li>
 } else if ( @node.Level == 5 )
 {
    <li @activeClass><a href="@url"@target>@( @node.menuLabel != "" ? @node.menuLabel : @node.Name )</a></li>
 } else
 {
  @* Ignore *@   
 }
}

    @if ( @Model.NodeById(@toNode).Level > 1 )
    {
      @traverse( @Model.NodeById(@toNode).AncestorOrSelf(2), @Model.NodeById(@toNode) )
    }



// navigation-navbar-title.cshtml

@using umbraco.MacroEngines
@using umbraco.MacroEngines.Library
@inherits umbraco.MacroEngines.DynamicNodeContext
@{
string linkUrl = "";
string linkLabel = "";
dynamic nodeId;

int toNode = @Model.Id;
if (!int.TryParse(Request.QueryString["r"], out toNode)) {
	toNode = @Model.Id;}
}

@if (Model.NodeById(@toNode).AncestorOrSelf("SectionPage") != null){
	nodeId = @Model.NodeById(@toNode).AncestorOrSelf("SectionPage");
}
else{
	nodeId = @Model.NodeById(@toNode).AncestorOrSelf("DeptHome");
}

@{linkUrl = nodeId.Url;}

@if(nodeId.HasValue("menuLabel")){
	linkLabel = nodeId.menuLabel;
}
else{
	linkLabel = nodeId.Name;
}
@if (Model.NodeTypeAlias != "DeptHome" && Model.NodeTypeAlias != "SectionPage") {
	<a class="navbar-link" href="@linkUrl">@Html.Raw(@umbraco.library.ReplaceLineBreaks(@linkLabel))</a>
	<hr/>
}

```



<img src='/images/navigation/side_nav.png'/>

## Side navigation mobile

<img src='/images/navigation/mobile-nav.png'/>

## Footer
Please refer to Home Page > Footer for the complete documentation on the navigation in the footer.

<aside class="notice">To Edit in Umbraco:</aside>
- Settings > Templates > Earlham
