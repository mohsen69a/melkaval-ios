# Uncomment the next line to define a global platform for your project
platform :ios, '15.0'

target 'ملک اول' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Add the pod for Firebase Cloud Messaging
  pod 'Firebase/Messaging'

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '15.0'
      # خط زیر برای غیرفعال کردن امضای کد اضافه شده است
      config.build_settings['CODE_SIGNING_ALLOWED'] = 'NO'
    end
  end
end