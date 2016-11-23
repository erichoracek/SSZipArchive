platform :ios, '8.0'

plugin 'cocoapods-rome'

target 'Rome' do
    pod 'SSZipArchive'
end

use_frameworks!

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['ENABLE_BITCODE'] = 'NO'
      config.build_settings['APPLICATION_EXTENSION_API_ONLY'] = 'YES'
    end
  end
end
