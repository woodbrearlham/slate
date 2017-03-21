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

<aside class="notice">To Edit in Umbraco:</aside>

- Settings > Templates > Earlham > Home

## Be An Earlhamite
<img src='/images/homepage/be-an-earlhamite.gif' />

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

### Footer Links

### Social Links
