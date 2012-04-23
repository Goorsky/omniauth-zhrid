# OmniAuth::zhrID 

Provides strategies for authenticating to providers using the zhrID standard. (http://id.zhr.pl)

## Installation

    gem 'omniauth-zhrid', :git => 'git@github.com:Goorsky/omniauth-zhrid.git'

## Stand-Alone Example

Use the strategy as a middleware in your application:

    require 'omniauth-zhrid'

    use Rack::Session::Cookie
    use OmniAuth::Strategies::zhrID

Then simply direct users to `/auth/open_id` to prompt them for their zhrID identifier. 

Read this tutorial and include zhrID authentication in your Rails 3 app: http://asciicasts.com/episodes/241-simple-omniauth

## OmniAuth Builder

If zhrID is one of several authentication strategies, use the OmniAuth Builder:

    require 'omniauth-zhrid'

    use OmniAuth::Builder do
      provider :zhr_id
    end

## License

Copyright (c) 2011 Michael Bleigh and Intridea, Inc., zhrID mods by Goorsky 

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
