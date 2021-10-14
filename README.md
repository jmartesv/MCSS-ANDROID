[![](http://docs.getmcss.com/img/logo_MCSS_pink.37f6be9a.svg)](https://www.getmcss.com)

# OVERVIEW
MCSS (Mobile Cascade Style Sheet) is a new technology library based to speed up the development of native mobile apps. MCSS describes how the views and the different components are to be displayed on the mobile devices. MCSS saves a lot of work and time, it can control the layout of multiple views all at once.

MCSS is not a hybrid technology, applications developed using MCSS continue being native, you can use your favorite IDE, XCode, Android Studio, Eclipse, etc. Just connecting this powerful library to your project ([how to install MCSS on your application project](https://docs.getmcss.com/installation-swift)) and doing a short implementation, your app will take the design described in the .mcss files.

Once you create a .mcss file, residing either on an external URL or stored locally in your project, the library will apply the instructions of your .mcss file to the different views and components. Just like CSS works on an HTML website. ([Read about the properties and components supported by MCSS](https://docs.getmcss.com/selectors)).

# WHY MCSS?

- Reduce native mobile app development by more than 40%.

- Can create complex designs and replicate them an infinite amount of times by just one line of code.

- No need to be an expert mobile developer to create a great looking app.

- Easy to maintain and update the app across the codebase and app store on iOS and Android.

- Helps provide the same design and aesthetics for iOS and Android version.

### Just like CSS is to HTML, MCSS is to Swift for iOS and Java for Android.

- MCSS Provide developers with a way to connect the components in each view of a mobile app with a set of stylesheets where they can write rules to control the design of the whole application.

- As the MCSS File (Stylesheet) can be connected via URL, the developers can update the design of applications in production skiping the process of submiting new versions to the app stores. 

# HOW TO INSTALL

### Gradle Package Manager:

1.  En tu proyecto de Android Studio abre el archivo build.gradle del proyecto, agrega el siguiente el siguiente fragmento de codigo:
		allprojects {
			repositories {
				maven { url 'https://jitpack.io' }
			}
		}

2.  Abre el archivo build.gradle del modulo, agrega el siguiente el siguiente fragmento de codigo:
		dependencies {
			implementation 'com.github.MCSSLIB : MCSS-ANDROID:1.0.0'
		}    ```
Si tu proyecto usa legacy debes importar la libreria de android support de MCSS:
		dependencies {
			implementation 'com.android.support:design : 28.0.0'
			implementation 'com.github.MCSSLIB : com.github.MCSSLIB:MCSS-ANDROID-LEGACY : 1.0.0'
		}


### Manual installation:

1.  Descarga la libreria mcss-android-release.aar  del repositorio https://github.com/MCSSLIB/MCSS-ANDROID o https://github.com/MCSSLIB/MCSS-ANDROID-LEGACY si tu proyecto usa Android Support. Tambien puedes clonar el proyecto usando git con el siguiente comando:

    ```
    git clone https://github.com/MCSSLIB/MCSS-ANDROID 
    ```

1.  En el modulo principal de tu proyecto de Android Studio crea una carpeta llamada libs.

2. Copia la libreria mcss-android-release.aar que acabas de descargar en la carpeta libs.

3.  En tu proyecto de Android Studio abre el archivo build.gradle del proyecto, agrega el siguiente el siguiente fragmento de codigo:
		allprojects {
			repositories {
				flatDir {
					dirs 'libs'
				}
			}
		}

4.  Abre el archivo build.gradle del modulo, agrega el siguiente el siguiente fragmento de codigo:
		dependencies {
			implementation files('libs/mcss-android-release.aar')
		}  

# COPYRIGHT & LICENSE
© 2021 MCSS | getmcss.com | Do Genius On. All rights reserved | Patent pending 

[MCSS License](https://www.getmcss.com/end-user-license).