# Dapplo.ActiveDirectory
A library which helps you with Active Directory access

Although it's not hard to access the Active Directory from .NET, sometimes a little bit of help is nice.

The idea is that you can build queries via a fluent API, and have some shortcuts available.

Fluent API:
	var query = QueryBuilder.And().UserCategory().Compare(UserProperties.Username, Environment.UserName);
Shortcut:
	var query = QueryBuilder.UsernameFilter(Environment.UserName);
