# Uncomment this line to define a global platform for your project
platform :ios, '10.0'

def shared_pods
    # Comment this line if you're not using Swift and don't want to use dynamic frameworks
    use_frameworks!
    # Pods for trid
    #Common
    pod 'SDWebImage'
    pod 'IQKeyboardManagerSwift'
    pod 'FontAwesomeKit'
    pod 'Toast-Swift'
    pod 'TTRangeSlider'
    #AutoLayout
    pod 'PureLayout'
    #Google
    #pod 'GoogleSignIn'
    pod 'GoogleMaps'
    pod 'Google-Mobile-Ads-SDK'
    #gmail
    pod 'GoogleAPIClientForREST/Gmail'
    #Hyperlink label
    pod 'TTTAttributedLabel'
    #Network
    pod 'Alamofire'
    #Json
    pod 'SwiftyJSON'
    
    #Admob
    #pod 'Google-Mobile-Ads-SDK'
    
    #loading
    pod 'MBProgressHUD'
end

#pro
target 'trid-dev' do
    shared_pods
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings["IPHONEOS_DEPLOYMENT_TARGET"] = "14.0"
    end
  end
  
  
end
