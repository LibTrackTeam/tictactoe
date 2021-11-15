source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '12.0'
use_frameworks!
inhibit_all_warnings!

target 'DTSocketTicTacToe' do
  pod 'CocoaAsyncSocket'

  post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '12.0'
        config.build_settings['DEBUG_INFORMATION_FORMAT'] = 'dwarf'
        config.build_settings['LD_NO_PIE'] = 'NO'
      end
    end
  end
end

