# Circular Gallery

A WebGL infinite circular gallery using OGL.

## Installs

```bash
npm install ogl
```

## Usage

```jsx
import CircularGallery from './CircularGallery';

const items = [
  { image: 'path/to/img1.jpg', text: 'Image 1' },
  { image: 'path/to/img2.jpg', text: 'Image 2' },
  // ...
];

const Example = () => {
  return (
    <div style={{ height: '600px' }}>
      <CircularGallery 
        items={items}
        bend={3}
        textColor="#ffffff"
        borderRadius={0.05}
      />
    </div>
  );
};

export default Example;
```

## Props

| Prop | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| `items` | `array` | `[]` | Array of objects with `image` (URL) and `text` properties. |
| `bend` | `number` | `3` | Curvature intensity of the gallery. |
| `textColor` | `string` | `'#ffffff'` | Color of the caption text. |
| `borderRadius` | `number` | `0.05` | Border radius of the images (0-1). |
| `font` | `string` | `'bold 30px Figtree'` | Font string for text captions. |
| `scrollSpeed` | `number` | `2` | Speed of scroll interaction. |
