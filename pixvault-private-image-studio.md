# Portfolio Project Data — PixVault - Private Image Studio

- **Category:** `desktop-mobile` (`Desktop App`)
- **Category Label:** `Desktop App`
- **Accent Color:** `amber`
- **Target Assets Folder:** `public/images/projects/pixvault_private_image_studio/`
- **Required Local Images:** `banner.webp`, `image01.webp` .. `image13.webp`

## TypeScript Data (`ProjectCaseStudy`)

```typescript
{
  "id": "pixvault-private-image-studio",
  "code": "PRO-55 // APP-09",
  "title": "PixVault - Private Image Studio",
  "category": "desktop-mobile",
  "categoryLabel": "Desktop App",
  "year": "2025",
  "status": "Completed",
  "accentColor": "amber",
  "repoUrl": "https://github.com/weztcy/PixVault-Private-Image-Studio",
  "license": "MIT License",
  "banner": "/images/projects/pixvault_private_image_studio/banner.webp",
  "summary": "Privacy-first offline Python and PySide6 desktop studio for multi-core batch image conversion, compression, ICC color, and metadata stripping.",
  "projectDescription": "PixVault is an offline Python and PySide6 desktop studio that converts, compresses, resizes, crops, transforms, and optimizes images locally across 10 output formats with ICC color management, 16/32-bit encoding, metadata stripping, and multi-core batch processing.",
  "architectureSummary": "PySide6 UI dispatches jobs via QThread and ProcessPoolExecutor workers through a deterministic ImagePipeline into format encoders and atomic JSON history.",
  "techStack": [
    "Python",
    "PySide6",
    "Pillow",
    "NumPy",
    "pillow-heif",
    "pillow-avif-plugin",
    "rawpy",
    "tifffile",
    "svgwrite",
    "PyInstaller"
  ],
  "telemetryMatrix": {
    "projectType": "Local Desktop Image Processing Studio",
    "targetPlatform": "Windows 10 / 11 (x64 Executable)",
    "primaryDomain": "Offline Media & Privacy Engineering",
    "architecturePipeline": "PySide6 -> ProcessPoolExecutor -> Encoders",
    "testingAndAudit": "Verified",
    "projectStatus": "Completed",
    "projectYear": "2025"
  },
  "desktopMobileProjectInfo": {
    "applicationType": "Native Desktop Image Studio",
    "targetPlatform": "Windows Desktop",
    "developmentStatus": "Completed",
    "developmentYear": "2025",
    "applicationCategory": "Offline Media Processing & Privacy"
  },
  "desktopMobileBackground": "Photographers, developers, and business teams frequently rely on browser-based converters that require uploading sensitive photos, RAW assets, or documents with embedded GPS and EXIF metadata to third-party servers, creating privacy risks, bandwidth bottlenecks, and weak control over bit depth or ICC color.",
  "desktopMobileProblemStatements": [
    {
      "title": "Privacy Exposure in Online Image Converters",
      "description": "Cloud-based conversion tools force users to upload private images, GPS coordinates, and camera metadata to remote servers without verifiable retention guarantees.",
      "issueCode": "ISSUE_01"
    },
    {
      "title": "Single-Threaded Bottlenecks on Large Batches",
      "description": "Basic desktop utilities block the UI thread or process files sequentially, stalling workflows when converting or compressing thousands of high-resolution images.",
      "issueCode": "ISSUE_02"
    },
    {
      "title": "Limited Bit Depth and ICC Color Fidelity",
      "description": "Standard image libraries strip or downgrade 16-bit PNGs, 32-bit float TIFFs, and embedded ICC profiles during conversion and print-density adjustments.",
      "issueCode": "ISSUE_03"
    },
    {
      "title": "Output Filename Collisions in Bulk Exports",
      "description": "Batch exports targeting shared destination directories risk silently overwriting files or suffering race conditions when worker processes write concurrently.",
      "issueCode": "ISSUE_04"
    }
  ],
  "desktopMobileObjectives": [
    {
      "title": "Zero-Upload On-Device Execution",
      "description": "Keep 100% of image decoding, processing, encoding, and activity logging offline on the user's machine with zero external API or cloud dependencies.",
      "targetTag": "TARGET_01"
    },
    {
      "title": "Multi-Core Parallel Batch Throughput",
      "description": "Distribute image pipelines across all logical CPU cores via ProcessPoolExecutor while keeping the PySide6 interface responsive with QThread signals.",
      "targetTag": "TARGET_02"
    },
    {
      "title": "Professional Format and Color Precision",
      "description": "Support 10 output formats including 8/16-bit PNG, 8/16/32-bit TIFF, HEIC, AVIF, and ICC profile transformations across sRGB, Adobe RGB, Display P3, and CMYK.",
      "targetTag": "TARGET_03"
    },
    {
      "title": "Collision-Free Export and Atomic History",
      "description": "Pre-allocate unique output paths in memory before batch execution and persist job audit logs safely using atomic temporary-file JSON replacement.",
      "targetTag": "TARGET_04"
    }
  ],
  "desktopMobileFeatures": [
    {
      "title": "Multi-Format Conversion Studio",
      "description": "Imports 14 image formats including RAW and SVG and exports to JPEG, PNG, WebP, AVIF, GIF, SVG, BMP, TIFF, HEIC, and ICO with format-specific encoder controls.",
      "badge": "CONVERSION"
    },
    {
      "title": "Quality and Target-Size Compression",
      "description": "Optimizes JPEG, PNG, WebP, and TIFF outputs via quality sliders or iterative KB/MB target-size reduction with size, balanced, and quality priority steps.",
      "badge": "OPTIMIZATION"
    },
    {
      "title": "Precision Resize, Crop, and Transform",
      "description": "Provides six resize strategies with Lanczos resampling, four crop modes including custom coordinates and aspect ratios, and rotation or flip transformations.",
      "badge": "GEOMETRY"
    },
    {
      "title": "ICC Color Space and High Bit-Depth Engine",
      "description": "Transforms images across bundled sRGB, Adobe RGB, Display P3, FOGRA39 CMYK, and Grayscale profiles and writes 16-bit PNG and 32-bit float TIFF files.",
      "badge": "COLOR_DEPTH"
    },
    {
      "title": "Granular Metadata Privacy Stripping",
      "description": "Wipes all embedded metadata or selectively removes EXIF, GPS tags, maker notes, XMP, IPTC, ICC profiles, software, and copyright fields prior to export.",
      "badge": "PRIVACY"
    },
    {
      "title": "Multi-Core Batch Queue and History Center",
      "description": "Processes up to thousands of images concurrently across CPU cores with real-time progress, immediate cancellation, and a searchable local JSON audit log.",
      "badge": "BATCH_ENGINE"
    }
  ],
  "desktopMobileInterfaceShowcase": [
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image01.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image02.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image03.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image04.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image05.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image06.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image07.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image08.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image09.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image10.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image11.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image12.webp"
    },
    {
      "imageUrl": "/images/projects/pixvault_private_image_studio/image13.webp"
    }
  ],
  "desktopMobileUserFlow": {
    "summary": "Users select an operation from the sidebar, drag files or folders into the collection workspace, inspect image metadata, tune encoder and output folder settings, and run multi-core local processing with live progress tracking and searchable export history.",
    "steps": [
      {
        "step": "01",
        "title": "Select Operation Workspace",
        "description": "Choose Convert, Compress, Resize, Crop, Transform, DPI, Metadata, Color Space, or Bit Depth from the sidebar to load the matching QStackedWidget workspace.",
        "actorOrNode": "User / Sidebar UI"
      },
      {
        "step": "02",
        "title": "Import and Inspect Media Queue",
        "description": "Drag and drop files or scan folders recursively, then inspect image thumbnails, resolution, file size, color mode, and bit depth locally.",
        "actorOrNode": "UI Thread / Pillow Inspector"
      },
      {
        "step": "03",
        "title": "Configure Format and Destination",
        "description": "Select the target format, tuning parameters, and default OneDrive/Pictures or custom export folder while NamingEngine prepares unique output paths.",
        "actorOrNode": "OutputSelector / NamingEngine"
      },
      {
        "step": "04",
        "title": "Execute Multi-Core Batch Pipeline",
        "description": "BatchService spawns a QThread and ProcessPoolExecutor pool that runs ImagePipeline stages and format encoders in parallel with live progress and cancellation.",
        "actorOrNode": "WorkerThread / ProcessPoolExecutor"
      },
      {
        "step": "05",
        "title": "Record Atomic History and Review",
        "description": "Main process batches completed or failed job metadata into local history.json via atomic temporary-file replacement for inspection in the History Center.",
        "actorOrNode": "HistoryManager / Local JSON"
      }
    ]
  },
  "desktopMobileArchitecture": {
    "summary": "PixVault implements a modular layered desktop architecture connecting PySide6 UI pages and service facades to a QThread and ProcessPoolExecutor batch engine, deterministic ordered processors, 10 format encoders, and atomic local JSON history persistence.",
    "layers": [
      {
        "name": "Presentation Layer",
        "role": "Renders the dark studio window, sidebar navigation, stacked tool pages, preview canvas, and live progress controls.",
        "tech": "PySide6",
        "components": ["MainWindow", "Sidebar", "Workspace", "OutputSelector"]
      },
      {
        "name": "Service & Concurrency Layer",
        "role": "Validates inputs, manages QThread lifecycle, and dispatches parallel tasks across logical CPU cores via ProcessPoolExecutor.",
        "tech": "Python Multiprocessing",
        "components": ["ImageService", "BatchService", "HistoryService", "WorkerThread", "BatchWorker"]
      },
      {
        "name": "Core Processing Pipeline",
        "role": "Normalizes raster or Qt-rendered SVG images and executes operations in deterministic sequence from resize through metadata stripping.",
        "tech": "Pillow & NumPy",
        "components": ["ImagePipeline", "SVGRenderer", "ColorSpaceProcessor", "BitDepthProcessor", "MetadataProcessor"]
      },
      {
        "name": "Export & Persistence Layer",
        "role": "Resolves collision-free filenames, delegates encoding across 10 format modules, and writes atomic JSON history logs.",
        "tech": "Local JSON & Codecs",
        "components": ["Exporter", "NamingEngine", "EncoderManager", "PNGEncoder", "TIFFEncoder", "HistoryManager"]
      }
    ]
  },
  "desktopMobileDataManagement": {
    "storageType": "Atomic Local JSON Store & Bundled ICC Files",
    "stateEngine": "PySide6 Qt Signals & Stacked Widget State",
    "offlineSyncStrategy": "100% Offline Local Execution (No Cloud Sync)",
    "cachingMechanism": "In-Memory Filename Reservation & Batch History Buffering"
  },
  "desktopMobilePlatformImplementation": [
    {
      "title": "Windows Frozen Executable Packaging",
      "description": "PyInstaller spec bundles native pillow-heif DLLs, pillow-avif binaries, bundled ICC color profiles, and application icons into a standalone windowed PixVault.exe binary.",
      "badge": "PACKAGING"
    },
    {
      "title": "Multi-Core Process Isolation & Plugin Bootstrapping",
      "description": "BatchWorker initializes HEIF and AVIF Pillow openers inside every child worker process, handles immediate process termination on cancel, and falls back to sequential mode if spawning is restricted.",
      "badge": "CONCURRENCY"
    },
    {
      "title": "Custom 16-Bit PNG and 32-Bit TIFF Writers",
      "description": "Bypasses Pillow's 8-bit multichannel limit with a custom CRC32/zlib chunk PNG writer for 16-bit RGB/RGBA/Grayscale and tifffile/NumPy export for 32-bit float TIFFs.",
      "badge": "LOW_LEVEL_IO"
    },
    {
      "title": "Windows Environment & AppData Path Resolution",
      "description": "Automatically resolves OneDrive or Pictures export folders and stores frozen executable history under %APPDATA%\\PixVault\\history.json with a headless --selftest diagnostic runner.",
      "badge": "OS_INTEGRATION"
    }
  ],
  "desktopMobileTechSpecs": {
    "programmingLanguage": "Python",
    "framework": "PySide6",
    "localStorage": "Local JSON"
  },
  "desktopMobilePlatformSpecs": {
    "targetPlatform": "Windows Desktop",
    "packageFormat": "Standalone EXE Bundle",
    "targetArchitecture": "64-bit x64",
    "buildFootprint": "78.5 MB Executable"
  }
}
```
