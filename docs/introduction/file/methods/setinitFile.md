Use this method to open a file when the viewer starts using a URL or server-side Windows path.

### Syntax

```typescript
RxCore.setinitFile(fileurl)
```

### Parameters

- `fileurl`: **string** — URL address or full server-side Windows path to a file to open in the viewer. This can be either a string or an object with the following properties:
  - `fileurlobj.filename`: **string** — A string containing the URL or path of the file to open.
  - `fileurlobj.mime`: **string** — A string containing the MIME type for the type of file to open or null.
  - `fileurlobj.cacheid`: **string** — A string containing a unique name to use for the cache entry or null.
  - `fileurlobj.displayname`: **string** — A string that is used as the document file name or null.

### Returns

- **NA** — This method does not return a value.