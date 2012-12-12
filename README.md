SolrPatches
===========

Repo containing patches for the Magento Enterprise integration with Solr.

Patches Provided
------------------

The following patch files have been provided:
* config.xml.patch:
	* File: app\code\core\Enterprise\Search\etc\config.xml
	* Bug: Currently solr will perform a complete index when started through the adminhtml but will miss searchable attributes when the index is started via the command-line,

* Abstract.php.patch
	* File: app\code\core\Enterprise\Search\Model\Adapter\Abstract.php
	* Bug: Currently a notice is raised when an attribute combination does not set $preparedValue.

* Service.php.patch
	* File: lib\Apache\Solr\Service.php
	* Bug: To fix issue where the ping function returns nothing from our server

author: David Manners, 12/2012
contact: http://www.sitewards.com