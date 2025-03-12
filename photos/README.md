# Minimalistic Photo Gallery

This is a static minimalistic photo gallery for your personal website. It's designed to display your photos organized into albums.

## How to Use

### Album Structure

- Each album should have its own folder inside the `photos` directory
- Each album folder should contain:
  - The photos you want to display
  - Thumbnails of those photos (optional but recommended)
  - A `photos.json` file describing the photos

### Adding a New Album

1. Create a new folder inside the `photos` directory (e.g., `photos/vacation`)
2. Add your photos to this folder
3. Create thumbnails for your photos (optional but recommended)
4. Create a `photos.json` file listing all photos in the album (see format below)
5. Add the album to `albums.json` in the main `photos` directory

### photos.json Format

```json
[
  {
    "filename": "photo1.jpg",
    "thumbnail": "thumb_photo1.jpg",
    "title": "Photo Title",
    "description": "Photo description"
  },
  {
    "filename": "photo2.jpg",
    "thumbnail": "thumb_photo2.jpg",
    "title": "Another Photo",
    "description": "Another description"
  }
]
```

If thumbnails are not provided, the original image will be used as the thumbnail.

### albums.json Format

```json
[
  {
    "title": "Album Title",
    "folder": "album_folder_name",
    "coverImage": "cover.jpg",
    "description": "Album description"
  },
  {
    "title": "Another Album",
    "folder": "another_album_folder",
    "coverImage": "cover.jpg",
    "description": "Another album description"
  }
]
```

The `coverImage` should be a photo in the album folder that will be used as the album cover.

## Image Tips

- For best performance, resize your images before adding them to the gallery
- Recommended sizes:
  - Full-size images: Max width/height of 1920px
  - Thumbnails: Max width/height of 400px
- Use JPEG format for photos for better compression
