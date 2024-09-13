# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'
platform :ios, '14.0'

install! 'cocoapods', :deterministic_uuids => false, :warn_for_multiple_pod_sources => false, :warn_for_unused_master_specs_repo => false

target 'application_ios' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  #swift
  # Pods for application_ios
  pod 'GoogleMaps'
  
  pod 'FirebaseCore'
  pod 'FirebaseAuth'
  pod 'FirebaseDatabase'
  pod 'FirebaseMessaging'
  pod 'FirebaseStorage'
  
  pod 'FBSDKCoreKit'
  pod 'FBSDKLoginKit'
  
  pod 'Alamofire'
  pod 'DGActivityIndicatorView'
  pod 'SDWebImage'
  
  pod 'SSZipArchive'
  pod 'TouchJSON'
  pod 'GDataXML-HTML'
  pod 'SQLite.swift/SQLCipher'
  pod 'AESCrypt'
  pod 'CryptoSwift'
  pod 'NSHash'
  target 'application_iosTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'application_iosUITests' do
    # Pods for testing
  end

  post_install do |installer|
      installer.generated_projects.each do |project|
          project.targets.each do |target|
              target.build_configurations.each do |config|
                  config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
              end
          end
      end
  end
  
end
