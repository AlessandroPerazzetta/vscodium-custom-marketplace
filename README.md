# VSCodium custom marketplace

Change VSCodium from osvx to ms marketplace



To change from osvx defined in product.json extensionsGallery, now simpy create a new product.json under user config VSCodium directory:



```bash
mkdir -p ~/.config/VSCodium/
vi ~/.config/VSCodium/product.json
```

Add the following lines:

```json
{
  "nameShort": "Visual Studio Code",
  "nameLong": "Visual Studio Code",
  "extensionsGallery": {
    "serviceUrl": "https://marketplace.visualstudio.com/_apis/public/gallery",
    "cacheUrl": "https://vscode.blob.core.windows.net/gallery/index",
    "itemUrl": "https://marketplace.visualstudio.com/items"
  }
}
```

Save and start VSCodium, check if extension marketplace now link to new marketplace.
