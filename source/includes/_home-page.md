#Home Page

The homepage received a refresh Jan of 2017.

## Hero Video (Macro)
```html
<script src="/scripts/jquery.mb.YTPlayer.min.js"></script>

<style>
	.heading-main {
	font-family: 'YWFTPakt';
    font-size: 34pt;
    line-height: 1.2em;
    text-transform: uppercase;
    text-align: left;
    margin: 0;
		color: #FFF;
	}
.heading {
	    border: 2px solid white;
    padding: 20px;
}
</style>
<!--Video Section-->
<section class="content-section video-section" >
	<div class="pattern-overlay">
    <a id="bgndVideo" class="player" data-property="{
      videoURL:'https://www.youtube.com/watch?v=whwhNrfcqZU',
      containment:'.video-section',
      quality:'large',
      autoPlay:true,
      mute:true,
      opacity:1,
      loop:true
    }">bg</a>
    <div class="callout-container">
      <a style="cursor:pointer;" class="video-modal-toggle"><div class="row"></div></a>
    </div>
  </div>
  </div>
</section>

			<script>
			$(document).ready(function () {

				$(".player").mb_YTPlayer({
					'ratio':'auto',
					'optimizeDisplay':'true',
					'align': 'top,center',
					'autoPlay':'true',
					'gaTrack': 'false',
				});

				$('.video-modal-toggle').on('click', function(event){
					ga('send', 'event', 'homepage-click', 'video-modal', 'Nowhere is the world closer');
				});

});
			</script>
<!--Video Section Ends Here-->

```
<img src='/images/homepage/hero-video.png'/>

<aside class="notice">To Edit in Umbraco:</aside>
- Developer > Scripting Files > video-carousel.cshtml
- Macro Alias: Feature-VideoCarousel
- Update: v="" in data-property

## Text Carousel
```html
<section id="quotes" data-anchor="quotes" class="module callout-container fp-auto-height">
    <div class="module-inner container">
        <div id="text-carousel" class="carousel slide" data-ride="carousel" data-wrap="true" data-keyboard="true">
          <div class="row">
              <ol class="carousel-indicators">
                  <li data-target="#text-carousel" data-slide-to="0" class="active"></li>
                  <li data-target="#text-carousel" data-slide-to="1"></li>
                  <li data-target="#text-carousel" data-slide-to="2"></li>
                  <li data-target="#text-carousel" data-slide-to="3"></li>
              </ol>
          </div>

          <!-- Wrapper for slides -->
          <div class="row">
              <div class="col-md-offset-2 col-md-8">
                <div class="carousel-inner">
                  <div class="item active">
                    <div class="carousel-content">
                      <div>
                      <h4>Learning Together</h4>
                      <p>Professors and peers will challenge and support you to excel in the classroom, the laboratory, the field and during off-campus programs. Wherever you go and whatever you study, you’ll enjoy questioning, exploring and discovering together.</p>
                      </div>
                    </div>
                  </div>
                  <div class="item">
                    <div class="carousel-content">
                      <div>
                      <h4>Preparing to Lead</h4>
                      <p>Develop the skills that corporate, political and educational leaders value most. Solve problems through true collaboration and refined communication. Analyze, create and adapt. Become the kind of leader you’d love to follow.</p>
                      </div>
                    </div>
                  </div>
                  <div class="item">
                    <div class="carousel-content">
                      <div>
                        <h4>Seeking Solutions</h4>
                        <p>Examine the world’s most complex challenges in new ways — from different angles and multiple lenses, and in real world settings — side by side with classmates and faculty from a range of backgrounds, viewpoints and perspectives.</p>
                      </div>
                    </div>
                  </div>
                    <div class="item">
                      <div class="carousel-content">
                          <div>
                            <h4>Being Mindful</h4>
                            <p>College should be more than just tests and papers. Discover how our deep commitment to integrity and respect for all people can shape the way you learn and live in a complex and diverse world.</p>
                          </div>
                      </div>
                    </div>
          </div><!-- /.carousel-inner -->
        </div>
      </div><!-- /.row -->
    </div><!-- /.carousel -->
  </div><!-- /.module-inner -->
</section><!-- /.module && /.callout-container -->

```
<img src='/images/homepage/text-carousel.gif'/>

Dependency | Description | Link to Doc
-------------- | -------------- | --------------
Slick Slider | JS/CSS | http://kenwheeler.github.io/slick/

<aside class="notice">To Edit in Umbraco:</aside>

- Settings > Templates > Earlham > Home

## Be An Earlhamite

```html
<section class="module join callout-container">
    	<div class="module-inner container ">
      		<div class="row text-center">
        		<div class="col-sm-12 col-md-8 col-md-offset-2 col-lg-offset-2 ">
      				<a href="/admissions" class="admissions-click">
		 				<div class="join-cta "><i class="fa fa-chevron-right"></i></div>
					</a>
      			</div>
    		</div>
    	</div>
	</section>

```

<img src='/images/homepage/be-an-earlhamite.gif' />

Image that points to the Admissions page.

<aside class="notice">To Edit in Umbraco:</aside>
- Settings > Templates > Earlham 


## EPIC section
<img src='/images/homepage/epic-section.png' />
## Infographic Stats
<img src='/images/homepage/info-graphic.gif' />

## News Hero
<img src='/images/homepage/news-hero.png' />
## News & Events Slider

```plaintext
  ga('send', 'event', 'homepage-click',
     'news-click', 'Earlham competition to offer $40K in seed capital for world-changing business ideas');
```
<img src='/images/homepage/news-events.gif' />

## Footer

```html
  <footer class="module footer">
      <div class="module-inner container">
        <div class="row">
			<div class="col-sm-3">
            <p><img alt="Earlham College Footer Logo" class="footer-logo" src="/media/2395270/footer-logo-2.png" width="40%" height="40%" align="right" />Earlham College, an independent, residential college, aspires to provide the highest-quality undergraduate education in the liberal arts, including the sciences, shaped by the distinctive perspectives of the Religious Society of Friends (Quakers).</p>
				<div class="footer-title">Translate Our Site</div>
					  <div id="google_translate_element"></div>
					<script type="text/javascript">
					    function googleTranslateElementInit() { new google.translate.TranslateElement({ pageLanguage: 'en', gaTrack: true, gaId: 'UA-20893274-1' }, 'google_translate_element'); }
					</script><script type="text/javascript" src="//translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>
          </div><!-- /.col-lg-3 -->
          <div class="col-sm-3">
            <ul>
				<li><a href="/academics/academic-calendar/">Academic Calendar</a></li>

<li><a href="/people/">Campus Directory</a></li>
              <li><a href="/maps/">Visiting Campus</a></li>
				<li><a href="http://www.earlhambookstore.com">Campus Store</a></li>
              <li><a href="/human-resources-and-business-operations/current-openings/">Employment</a></li>
              <li><a href="/consumer-information/">Consumer Information</a></li>
              <li><a href="/marketing-and-communications/website-feedback-form/">Website Feedback Form</a></li>
				<li><a href="/policies-and-handbooks/">Policies &amp; Handbooks</a></li>
				<li><a href="/news/">News Headlines</a></li>
				<li><a href="/events/">Events Calendar</a></li>
				<li><a href="/news/today/">Today@Earlham</a></li>
				<li><a href="http://library.earlham.edu">Earlham Libraries</a></li>
				<li><a href="/mail/">Earlham Email</a></li>
            </ul>
          </div><!-- /.col-lg-3 -->
          <div class="col-sm-3">
            <address>
              Earlham College<br>
              801 National Road West<br>
              Richmond, Indiana<br>
              47374-4095<br>
				1-765-983-1200 &mdash; Main Switchboard<br/>
				1-800-EARLHAM (327-5426) &mdash; Admissions<br/>
            </address>
            <div class="module social">
              <div class="module-inner">
                <a href="https://www.facebook.com/earlhamcollege" target="_blank" class="btn btn-facebook"><i class="icon-facebook icon-large"></i></a>
                <a href="https://twitter.com/earlham1847" target="_blank" class="btn btn-twitter"><i class="icon-twitter icon-large"></i></a>
                <a href="http://www.youtube.com/earlhamcollege" target="_blank" class="btn btn-youtube"><i class="icon-youtube icon-large"></i></a>
				<a href="http://instagram.com/earlhamcollege1847" target="_blank" class="btn btn-instagram"><i class="icon-instagram icon-large"></i></a>
				<a href="http://www.snapchat.com/add/earlhamcollege" title="snapchat" target="_blank" class="btn btn-snapchat"><i class="fa fa-snapchat-ghost" aria-hidden="true"></i></a>
                <a href="http://earlham.edu/news/rss/" target="_blank" class="btn btn-rss"><i class="icon-rss icon-large"></i></a>
              </div>
            </div>
          </div><!-- /.col-lg-3 -->
          <div class="col-sm-3">
				<iframe frameborder="0" scrolling="no" allowTransparency="true" width="150" height="166" src="https://cdn.yoshki.com/iframe/54732.html" style="border:0px; margin:0px; padding:0px; backgroundColor:transparent;"></iframe></p>
          </div><!-- /.col-lg-3 -->
        </div><!-- /.row -->
      </div><!-- /.footer-inner -->
    </footer><!-- /.footer -->
```

<img src='/images/homepage/footer.png'/>

### Footer Links

<ul>
<li><a href="#">Academic Calendar</a></li>
<li><a href="#">Campus Directory</a></li>
<li><a href="#">Visiting Campus</a></li>
<li><a href="#">Campus Store</a></li>
<li><a href="#">Employment</a></li>
<li><a href="#">Consumer Information</a></li>
<li><a href="#">Website Feedback Form</a></li>
<li><a href="#">Policies &amp; Handbooks</a></li>
<li><a href="#">News Headlines</a></li>
<li><a href="#">Events Calendar</a></li>
<li><a href="#">Today@Earlham</a></li>
<li><a href="#">Earlham Libraries</a></li>
<li><a href="#">Earlham Email</a></li>
</ul>


### Social Links

Social Medium | Link
-------------- | --------------
Facebook | https://www.facebook.com/earlhamcollege
Twitter | https://twitter.com/earlham1847
Instagram | http://instagram.com/earlhamcollege1847
SnapChat | http://www.snapchat.com/add/earlhamcollege
Youtube | http://www.youtube.com/earlhamcollege
RSS | http://earlham.edu/news/rss/

<aside class="notice">To Edit in Umbraco:</aside>
- Settings > Templates > Earlham