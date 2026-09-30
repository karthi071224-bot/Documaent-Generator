from dataclasses import dataclass, field
from typing import List, Dict, Any, Optional

@dataclass
class LegalDocumentChunk:
    chunk_id: str
    doc_id: str
    title: str
    jurisdiction: str
    section_number: str
    content: str
    metadata: Dict[str, Any] = field(default_factory=dict)
