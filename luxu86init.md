```shell
# start mysql server
mysql.server start --mysqlx=OFF # stop|restart

# get the port
netstat -ap tcp | grep -i "listen"

# create user
sudo mysql

msyql>
DROP USER IF EXISTS 'acore'@'localhost';
mysql>
CREATE USER 'acore'@'localhost' IDENTIFIED BY 'acore' WITH MAX_QUERIES_PER_HOUR 0 MAX_CONNECTIONS_PER_HOUR 0 MAX_UPDATES_PER_HOUR 0;
mysql>
GRANT ALL PRIVILEGES ON * . * TO 'acore'@'localhost' WITH GRANT OPTION;
mysql>
CREATE DATABASE `acore_world` DEFAULT CHARACTER SET UTF8MB4 COLLATE utf8mb4_unicode_ci;
mysql>
CREATE DATABASE `acore_characters` DEFAULT CHARACTER SET UTF8MB4 COLLATE utf8mb4_unicode_ci;
mysql>
CREATE DATABASE `acore_auth` DEFAULT CHARACTER SET UTF8MB4 COLLATE utf8mb4_unicode_ci;
mysql>
GRANT ALL PRIVILEGES ON `acore_world` . * TO 'acore'@'localhost' WITH GRANT OPTION;
mysql>
GRANT ALL PRIVILEGES ON `acore_characters` . * TO 'acore'@'localhost' WITH GRANT OPTION;
mysql>
GRANT ALL PRIVILEGES ON `acore_auth` . * TO 'acore'@'localhost' WITH GRANT OPTION;

/Users/xlu/Workspace/azerothcore/azeroth-server/bin/authserver
/Users/xlu/Workspace/azerothcore/azeroth-server/bin/worldserver


character level ${CharacterName} 70
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 4500 // Traveler's Backpack
additem ${CharacterName} 16853 // Lawbringer Chestguard
additem ${CharacterName} 16854 // Lawbringer Helm
additem ${CharacterName} 16855 // Lawbringer Legplates
additem ${CharacterName} 16856 // Lawbringer Spaulders
additem ${CharacterName} 16857 // Lawbringer Bracers
additem ${CharacterName} 16858 // Lawbringer Belt
additem ${CharacterName} 16859 // Lawbringer Boots
additem ${CharacterName} 16860 // Lawbringer Gauntlets
additem ${CharacterName} 19019 // Thunderfury, Blessed Blade of the Windseeker
additem ${CharacterName} 16471 // Marshal's Lamellar Gloves
additem ${CharacterName} 16472 // Marshal's Lamellar Boots
additem ${CharacterName} 16473 // Field Marshal's Lamellar Chestplate
additem ${CharacterName} 16474 // Field Marshal's Lamellar Faceguard
additem ${CharacterName} 16475 // Marshal's Lamellar Legplates
additem ${CharacterName} 16476 // Field Marshal's Lamellar Pauldrons
additem ${CharacterName} 18876 // Grand Marshal's Claymore
additem ${CharacterName} 21499 // Vestments of the Shifting Sands
additem ${CharacterName} 21663 // Robes of the Guardian Saint
additem ${CharacterName} 1604  // Chromatic Sword
additem ${CharacterName} 23999 // Honor Hold Tabard
additem ${CharacterName} 28367 // Greatsword of Forlorn Visions
additem ${CharacterName} 28765 // Stainless Cloak of the Pure Hearted
additem ${CharacterName} 32375 // Bulwark of Azzinoth
additem ${CharacterName} 32458 // Ashes of Al'ar
additem ${CharacterName} 35275 // Orb of the Sin'dorei
additem ${CharacterName} 35494 // Shroud of Winter's Chill
additem ${CharacterName} 35504 // Phoenix Hatchling
additem ${CharacterName} 40343 // Armageddon
additem ${CharacterName} 44606 // Toy Train Set

send money ${CharacterName} "money" "money" 999999999

update character_reputation set standing=42000 where faction=946;
```
