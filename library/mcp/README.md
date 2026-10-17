# MCP Server Library

**2 mục từ danh mục đã chốt**, đang theo dõi dưới dạng metadata. Cần review quyền truy cập, authentication và tính an toàn trước khi cài. Không lưu tokens/secrets trong repository Public.

[← Library](../README.md) · [catalog.csv](catalog.csv)

| Tên | Vai trò | Transport | Trạng thái |
| --- | --- | --- | --- |
| [GhidraMCP](https://github.com/LaurieWired/GhidraMCP) | MCP server tích hợp Ghidra để hỗ trợ reverse engineering | Cần xác minh theo README | Chưa thử |
| [FlowAgent / Power Automate Codex Ready](https://github.com/microsoft/power-platform-skills) | Bundle đã gửi: Node.js stdio MCP FlowAgent + 9 skills; upstream link là nguồn skills tham chiếu, không mặc định là source của FlowAgent | stdio Node.js (theo ZIP đã phân tích) | Đã phân tích ZIP, chưa thử |

**Phân biệt:** MCP server cung cấp công cụ cho agent; Agent Skill cung cấp hướng dẫn hành vi/kiến thức. Link upstream của Power Platform Skills **không được coi** là repository chính thức của FlowAgent trong ZIP đã tải lên.
