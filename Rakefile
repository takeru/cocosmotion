$:.unshift("/Library/RubyMotion/lib")
require 'motion/project'

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  app.name = 'cocosmotion'

  app.vendor_project( "vendor/cocos2d-iphone", :xcode,
    :xcodeproj => "cocos2d-ios.xcodeproj", :target => "cocos2d", :products => ["libcocos2d.a"],
    :headers_dir => "cocos2d")

  app.vendor_project "vendor/cocos2d-iphone/CocosDenshion/CocosDenshion", :static

  app.frameworks += ["OpenGLES", "OpenAL", "AVFoundation", "AudioToolbox", "QuartzCore"]
  app.libs << "/usr/lib/libz.dylib"

end
