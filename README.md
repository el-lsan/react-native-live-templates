# react-native-live-templates
Jetbrains Live Templates / Snippets for React Native.

Some basic react-native live templates for the Webstorm/Jetbrains IDE.

### Installation
Templates can be included by copying the React Native.xml to your [Templates](https://www.jetbrains.com/help/idea/sharing-live-templates.html) folder:  
OSX: ```~/Library/Preferences/IntelliJ IDEA<version>/templates```  
Windows: ```<your_user_home_directory>\.IntelliJ IDEA<version_number>\config\templates```

### Snippets:

// rncomp | Creates a new component and stylesheet
```js
/** 
 * $class_name_and_description$
 * @author $author_name$
 * created on $creation_date$
 */

import React, { Component } from 'react';
import { Platform, View, StyleSheet, Text, Image, AppRegistry } from 'react-native';

export default class $class_name$ extends Component <{}> {
		
	render() {
		return <view>$additional_views$$END$</view>;
	}
}

const styles = StyleSheet.create({
	// todo
});
```


// rnstyle | shortcut for creating a new stylesheet
```js
const styles = StyleSheet.create({
	$END$// todo
});
```

// rnregister | registers a component
```js
AppRegistry.registerComponent('$component_name$', () => App);
$END$
```

// rnpselect | shortcut for Plaform.select
```js
const $variable_name$ = Platform.select({
	ios: $ios_instructions$,
	android: $android_instructions$
});
$END$
```

---

ikbenpinda|a-chan, 2017
