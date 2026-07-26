```java
package dev.noonracc.me;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;
import java.util.List;

@RestController
@RequestMapping("/api/v1/about-me")
public class DeveloperController {

    @GetMapping
    public DeveloperProfile getProfile() {
        return DeveloperProfile.builder()
            .firstName("Stanisław")
            .lastName("Sołtysik")
            .role("Fullstack Developer")
            .coreTechnologies(List.of("Java", "SQL", "React"))
            .backPainStatus("Loading...")
            .build();
    }

    @GetMapping("/education")
    public EducationInfo getEducationInfo() {
        return EducationInfo.builder()
            .isStudying(true)
            .degree("Computer Science")
            .university("Polish-Japanese Academy of Information Technology")
            .build();
    }

    @GetMapping("/contact")
    public ContactInfo getContact() {
        return ContactInfo.builder()
            .email("soltysikstanislaw@wp.pl")
            .linkedIn("linkedin.com/in/stanislaw-soltysik-profile")
            .build();
    }
}
```

### 🛠 Tech Stack

#### ⚙️ Backend
<p align="left">
  <img src="https://img.shields.io/badge/Java-1E1E1E?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/Spring_Boot-1E1E1E?style=for-the-badge&logo=spring-boot&logoColor=white" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/SQL-1E1E1E?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL" />
</p>

#### 🌐 Frontend
<p align="left">
  <img src="https://img.shields.io/badge/React-1E1E1E?style=for-the-badge&logo=react&logoColor=white" alt="React" />
  <img src="https://img.shields.io/badge/JavaScript-1E1E1E?style=for-the-badge&logo=javascript&logoColor=white" alt="JavaScript" />
  <img src="https://img.shields.io/badge/HTML5-1E1E1E?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1E1E1E?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
</p>

#### 🔧 Tools & DevOps
<p align="left">
  <img src="https://img.shields.io/badge/Git-1E1E1E?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
  <img src="https://img.shields.io/badge/Docker-1E1E1E?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Linux-1E1E1E?style=for-the-badge&logo=linux&logoColor=white" alt="Linux" />
  <img src="https://img.shields.io/badge/Bash-1E1E1E?style=for-the-badge&logo=gnu-bash&logoColor=white" alt="Bash" />
</p>
