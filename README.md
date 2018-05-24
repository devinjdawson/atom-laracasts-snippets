# Sublime Text - Snippets  
This project is originally forked from vicgonvt/snippets.    

This is at least one set of the Laravel snippets that Jeffrey Way uses in his Sublime Editor for Laracasts. These snippets have been converted with the Atomizr plugin to use in Atom Text Editor. This tool is geared towards any person working with Laravel and its environment, or for anyone who is following along with Jeffrey Way's Laracasts and would like to work more efficiently.

# Installation  
To install the snippets in your Atom Editor, you will have to clone this repo into your own computer(s).  

In your terminal:  
```
cd ~/.atom/packages/
git clone git@github.com:devinjdawson/snippets.git
cd snippets
apm install
apm link .
```

This will create a directory called `snippets` which will contain all of the snippets.

That's it! It's that easy.

Contributions and suggestions welcomed!!!


# What's in the box

## PHP Class Methods

#### Public Method
+ Shortcut: `met`

```php
public function [METHOD_NAME]()
{
    //
}
```

#### Private Method
+ Shortcut: `pmet`

```php
private function [METHOD_NAME]()
{
    //
}
```

#### Protected Method
+ Shortcut: `prmet`

```php
protected function [METHOD_NAME]()
{
    //
}
```

#### Public Static Method
+ Shortcut: `smet`

```php
public static function [METHOD_NAME]()
{
    //
}
```

#### Construct Method
+ Shortcut: `cmet`

```php
public function __construct()
{
    //
}
```

## PHP Helpers

#### Die & Dump
+ Shortcut: `dd`
For those of us that use Laravel, dd() is missed when working outside the framework. Here is a workaround.

```php
die(var_dump($[VAR]));
```

## Laravel Views

#### Blade Variable Echo

Quick helper for outputting variables in blade templates.

```php
{{ $var }}
```

## Laravel Relationships

Laravel relationships are easy to write and now they take a second or two. Big thank you to Adam Wathan for the original idea on these. Modified a little bit for my personal preference. I mostly label my relationships to make sense regardless of my model's name. There is a stop at the method name, a second, optional, stop for the model's name and in some cases another stop to specify the table's field name.

#### BelongsTo
+ Shortcut: `belt`

```php
public function relationship()
{
    return $this->belongsTo(Relationship::class, 'field_name');
}
```

#### BelongsToMany
+ Shortcut: `belm`

```php
public function relationship()
{
    return $this->belongsToMany(Relationship::class, 'field_name');
}
```

#### HasMany
+ Shortcut: `hasm`

```php
public function relationship()
{
    return $this->hasMany(Relationship::class, 'field_name');
}
```

#### HasOne
+ Shortcut: `haso`

```php
public function relationship()
{
    return $this->hasOne(Relationship::class);
}
```

# Laravel Models

#### Fillable Fields Array
+ Shortcut: `fil`

```php
/**
 * @var array
 */
protected $fillable = ['FIELD'];

```

## PHPUnit

#### Test Method

Quick helper for scaffolding a new test method.

```php
public function testName()
{
    //
}
```
