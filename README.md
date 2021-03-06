# OneBike
An Android application that makes bike rides even more fabulous

# Importing the project into Android Studio

* Download and install Android Studio
	* Create an environment variable "ANDROID_HOME" to [path_to_android_studio_install]/sdk
	* Add to PATH, ANDROID_HOME/tools and ANDROID_HOME/platform-tools
* Open Android Manager with <code>android</code> command and install (or check if already installed)
	* Android 4.3 (API 18) -> SDK Platform
	* Extras
		* Google Play Services
		* Google Repository
		* Android Support Repository
		* Android Support Library
	* Tools
		* Android SDK Tools
		* Android SDK Platform-tools
		* Android SDK Build-tools
* Create a file `api_keys.properties` in the folder `src/OneBike/OneBike/src/main/res/raw` (create the folder if doesn't exist) :

<pre>
	An_API=###
</pre>

* Import the project into Android Studio:
	* Open Android Studio
	* Import Project
	* Select OneBike (src/OneBike)
	* Import project from external model: Gradle
	* Check Use auto-import and select Use gradle wrapper

That's it!

# Updating the JCDecaux contracts file

* Call the JCDecaux real time service:
GET https://api.jcdecaux.com/vls/v1/contracts HTTP/1.1

* Paste the result json in the `src/OneBike/OneBike/src/main/res/raw/contracts.json` file

# MIT License
This application is released under the MIT License. See the LICENSE file for more details.
