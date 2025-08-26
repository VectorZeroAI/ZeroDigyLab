# ZeroDigyLab
A mini AGI, capable of recursive reasoning and internal improovements.

---

Versioning/storage DB :

CREATE TABLE FileVersions (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  file_name TEXT NOT NULL,
  file_type TEXT,
  version_type TEXT NOT NULL,        -- 'p' or 'r'
  version_number INTEGER NOT NULL,
  content BLOB,
  change_notes TEXT,
  created_at DATETIME DEFAULT CURRENT_TIMESTAMP,
  UNIQUE(file_name, version_type, version_number)
);
