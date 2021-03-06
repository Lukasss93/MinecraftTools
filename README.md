# Minecraft Tools

[![Latest Stable Version](https://poser.pugx.org/lukasss93/minecraft-tools/v/stable)](https://packagist.org/packages/lukasss93/minecraft-tools)
[![Total Downloads](https://poser.pugx.org/lukasss93/minecraft-tools/downloads)](https://packagist.org/packages/lukasss93/minecraft-tools)
[![License](https://poser.pugx.org/lukasss93/minecraft-tools/license)](https://packagist.org/packages/lukasss93/minecraft-tools)
![PHP](https://img.shields.io/badge/php-%3E%3D5.6-green.svg)

> Minecraft Tools library for some basic API information.

Requirements
---------
* PHP >= 5.6
* Json Extension

Installation
---------
You can install this library with composer:

`composer require lukasss93/minecraft-tools`

Using
---------
```php
<?php
	use MinecraftTools\MinecraftTools;
	
	//Show the status of Mojang Services
	print_r( MinecraftTools::serviceStatuses() );
	
	//Get UUID from username
	print_r( MinecraftTools::getUUID('Lukasss93') );
	
	//Get username from UUID
	print_r( MinecraftTools::getUsername('UUID') );
	
	//Get name history from UUID
	print_r( MinecraftTools::getNameHistory('UUID') );
	
	//Add dashes to an UUID
	print_r( MinecraftTools::formatUUID('UUID') );
	
	//Remove dashes from UUID
	print_r( MinecraftTools::minifyUUID('UUID') );
	
	//Check if string is a valid UUID, with or without dashes
	print_r( MinecraftTools::isValidUUID('UUID') );
	
?>
```

Changelog
---------
All notable changes to this project will be documented [here](https://github.com/Lukasss93/minecraft-tools/blob/master/CHANGELOG.md).

### Recent changes
## [1.0]
- First release
