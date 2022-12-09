```
app
├── node_modules
│   └── @tigerconnect
│       ├── dep-a
│       │   ├── node_modules
│       │   │   └── @tigerconnect
│       │   │       └── dep-c
│       │   │           └── package.json => "version": "2.0.0"
│       │   └── package.json             => "dependencies": { "@tigerconnect/dep-c": "2.0.0" }
│       ├── dep-b
│       │   └── package.json             => "dependencies": { "@tigerconnect/dep-c": "1.0.0" }
│       └── dep-c
│           └── package.json             => "version": "1.0.0"
├── package-lock.json
└── package.json
```
