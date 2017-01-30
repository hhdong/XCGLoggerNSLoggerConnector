
use_frameworks!

target 'XCGLoggerNSLoggerConnector' do
    platform :ios, '9.0'
    pod 'XCGLogger', '>= 4'
    pod 'NSLogger', '>= 1.5'
end


target 'XCGLoggerNSLoggerConnector-OSX' do
    platform :osx, '10.12'
    pod 'XCGLogger', '>= 4'
    pod 'NSLogger', '>= 1.5'
end

post_install do |installer|
	installer.pods_project.targets.each do |target|
		target.build_configurations.each do |config|
			config.build_settings['SWIFT_VERSION'] = '3.0'
		end
	end
end
