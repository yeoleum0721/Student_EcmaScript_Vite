* student-es6-vite/
* ├── index.html
* ├── package.json  
* ├── vite.config.js
* └── src/
*     ├── main.js              # 메인 앱 로직
*     ├── modules/
*     │   ├── api.js           # API 통신 담당
*     │   ├── validation.js    # 유효성 검사 담당
*     │   └── ui.js            # UI 관리 담당
*     ├── utils/
*     │   └── helpers.js       # 유틸리티 함수들
*     └── css/
*         └── style.css        # 스타일시트

#### 1. 모듈 시스템 (ES6 Modules)        
```
// api.js에서 내보내기
export const apiService = {
    getStudents: async () => { ... }
}

// main.js에서 가져오기
import { apiService } from './modules/api.js'
import { validateStudent } from './modules/validation.js'