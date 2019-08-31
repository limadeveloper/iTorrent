platform :ios, '9.3'

target 'iTorrent' do
  use_frameworks!
  inhibit_all_warnings!

  # Pods for iTorrent
  pod 'Firebase/Core'
  pod 'Firebase/Performance'
  pod 'Fabric'
  pod 'Crashlytics'
  pod 'MarqueeLabel'
  pod 'Google-Mobile-Ads-SDK'

end

post_install do |installer|
	installer.pods_project.targets.each do |target|
		target.build_configurations.each do |config|
			config.build_settings['ENABLE_BITCODE'] = 'YES'
		end
	end
end