class Picturefill < Liquid::Tag

  def initialize(tag_name, input, tokens)
     super
     @image = input.split('|', 2).first
     @title = input.split('|', 2).last
  end

  def render(context)
    "<div data-picture data-alt=\"#{@title}\">
      <div data-src=\"img/#{@image}320.jpg\"></div>
      <div data-src=\"img/#{@image}320_x2.jpg\" data-media=\"(min-width: 320px) and (-webkit-min-device-pixel-ratio: 2.0)\"></div>
      <div data-src=\"img/#{@image}480.jpg\" data-media=\"(min-width: 480px)\"></div>
      <div data-src=\"img/#{@image}480_x2.jpg\" data-media=\"(min-width: 480px) and (-webkit-min-device-pixel-ratio: 2.0)\"></div>
      <div data-src=\"img/#{@image}768.jpg\" data-media=\"(min-width: 768px)\"></div>
      <div data-src=\"img/#{@image}768_x2.jpg\" data-media=\"(min-width: 768px) and (-webkit-min-device-pixel-ratio: 2.0)\"></div>
      <div data-src=\"img/#{@image}1024.jpg\" data-media=\"(min-width: 1024px)\"></div>
      <div data-src=\"img/#{@image}1024_x2.jpg\" data-media=\"(min-width: 1024px) and (-webkit-min-device-pixel-ratio: 2.0)\"></div>
      <div data-src=\"img/#{@image}1200.jpg\" data-media=\"(min-width: 1200px)\"></div>
      <div data-src=\"img/#{@image}1200_x2.jpg\" data-media=\"(min-width: 1200px) and (-webkit-min-device-pixel-ratio: 2.0)\"></div>
      <div data-src=\"img/#{@image}1600.jpg\" data-media=\"(min-width: 1600px)\"></div>
      <div data-src=\"img/#{@image}1600_x2.jpg\" data-media=\"(min-width: 1600px) and (-webkit-min-device-pixel-ratio: 2.0)\"></div>
      <!-- Fallback content for non-JS browsers. Same img src as the initial, unqualified source element. -->
      <noscript>
        <img src=\"img/#{@image}320.jpg\" alt=\"#{@title}\">
      </noscript>
    </div>"
  end

  Liquid::Template.register_tag "picturefill", self
end