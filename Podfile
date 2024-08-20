#platform :ios, '13.0'
#use_frameworks!
#
#target 'FinanceApp' do
#  pod 'TesseractOCRiOS'
#end


platform :ios, '13.0'
use_frameworks!

target 'FinanceApp' do
  pod 'TesseractOCRiOS'
end

post_install do |installer|
  installer.pods_project.build_configurations.each do |config|
    config.build_settings['EXCLUDED_ARCHS[sdk=iphonesimulator*]'] = 'arm64'
  end
end
