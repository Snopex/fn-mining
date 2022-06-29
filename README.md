# Discord
https://discord.gg/Ks2U2b4yhh

# fn-mining
Mining Script for QBCore

# Installation
Add the item to your qb-core/shared/item.lua

<pre class="notranslate"><code>-- Mining
	['mining_pickaxe'] 			     = {['name'] = 'mining_pickaxe', 				['label'] = 'Mining Pickaxe', 			['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_pickaxe.png', 			['unique'] = true, 			['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Classic\'s pickaxe for mining'},
	['mining_pan'] 			    	 = {['name'] = 'mining_pan', 					['label'] = 'Washing Pan', 				['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_pan.png', 				['unique'] = true, 			['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Classic\'s washing pan'},
	['mining_stone'] 			     = {['name'] = 'mining_stone', 					['label'] = 'Mined Stone', 				['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_stone.png', 			['unique'] = false, 		['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Mined Stone'},
	['mining_washedstone'] 			 = {['name'] = 'mining_washedstone', 			['label'] = 'Washed Stone', 			['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_washedstone.png', 		['unique'] = false, 		['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Wasted Stone'},
	['mining_ironfragment'] 		 = {['name'] = 'mining_ironfragment', 			['label'] = 'Iron Fragment', 			['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_ironfragment.png', 		['unique'] = false, 		['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Iron fragment from mining'},
	['mining_ironbar'] 				 = {['name'] = 'mining_ironbar', 				['label'] = 'Iron Bar', 				['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_ironbar.png', 			['unique'] = false, 		['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Iron Bar'},
	['mining_goldnugget'] 			 = {['name'] = 'mining_goldnugget', 			['label'] = 'Golden Nugget', 			['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_goldnugget.png', 		['unique'] = false, 		['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Golden nugget from mining'},
	['mining_goldbar'] 				 = {['name'] = 'mining_goldbar', 				['label'] = 'Gold Bar', 				['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_goldbar.png', 			['unique'] = false, 		['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Gold Bar'},
	['mining_copperfragment'] 		 = {['name'] = 'mining_copperfragment', 		['label'] = 'Copper Fragment', 			['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_copperfragment.png', 	['unique'] = false, 		['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Copper fragment from mining'},
	['mining_copperbar'] 			 = {['name'] = 'mining_copperbar', 				['label'] = 'Copper Bar', 				['weight'] = 500, 		['type'] = 'item', 		['image'] = 'mining_copperbar.png', 		['unique'] = false, 		['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Copper Bar'},

</code></pre>

For images move the images from the img folder to your inventory image folder qb-inventory/html/images

If you use another Drawtext like cd_drawtextui for example change the following in the client/main.lua 287 - 296

# Before DRAWTEXT

<pre class="notranslate"><code>exports['qb-core']:DrawText(Config.Text['MiningAlert'], 'left')

exports['qb-core']:DrawText(Config.Text['StartMining'],'left')
</code></pre>

# After

<pre class="notranslate"><code>TriggerEvent('cd_drawtextui:ShowUI', 'show', Config.Text['MiningAlert'])
		
TriggerEvent('cd_drawtextui:ShowUI', 'show', Config.Text['StartMining'])
</code></pre>

# You will also need to remove this line if you are using CD_Drawtextui Line 160

<pre class="notranslate"><code>exports['qb-core']:KeyPressed()
</code></pre>

# Preview Pictures

![68747470733a2f2f692e696d6775722e636f6d2f6d7530674e51432e6a706567](https://user-images.githubusercontent.com/103960355/176457374-0973c398-e127-45a9-9985-0ec204ccc724.jpg)
![68747470733a2f2f692e696d6775722e636f6d2f37674b653977452e6a706567](https://user-images.githubusercontent.com/103960355/176457431-a0f06a7b-80ba-4c72-ba3a-f4ab866261d1.jpg)
![68747470733a2f2f692e696d6775722e636f6d2f634761546733562e6a706567](https://user-images.githubusercontent.com/103960355/176457443-a6009514-cbbb-4410-a5dd-4ec6e707839b.jpg)
![68747470733a2f2f692e696d6775722e636f6d2f6d793232795a4c2e6a706567](https://user-images.githubusercontent.com/103960355/176457456-e6e8b9fb-cbd7-49fc-ab32-e8ee114e215d.jpg)
![68747470733a2f2f692e696d6775722e636f6d2f6655513631426c2e6a706567](https://user-images.githubusercontent.com/103960355/176457468-0135c3c1-8468-4351-a42d-6bd6a55e43e8.jpg)
![68747470733a2f2f692e696d6775722e636f6d2f564a436b3663782e6a706567](https://user-images.githubusercontent.com/103960355/176457480-b922baa0-56a0-46f1-a3e9-f3ec5b23de06.jpg)

# Discord
https://discord.gg/Ks2U2b4yhh



