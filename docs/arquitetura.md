# Arquitetura de Fluxo - BluaDiagnostics (Ecossistema Integrado)

```mermaid
graph TD
    A[Usuário/Paciente inicia o Chat] --> B[Acesso Automatizado: Chip de Monitoramento Biomédico]
    B --> C[Coleta de Sinais Vitais: Temp, Pressão, Batimentos, Glicose]
    C --> D[Motor de IA: Doctor Blua + Nurse Blua]
    
    D --> E{Cálculo de Risco Clínico}
    
    E -- ALTO RISCO: Dor no peito / Falta de Ar --> F[Interrupção Imediata + Alerta de Emergência Hospitalar]
    E -- MÉDIO RISCO: Taquicardia / Sinais Alterados --> G[Direcionamento para Agendamento Prioritário]
    E -- BAIXO RISCO: Sintomas Leves --> H[Direcionamento para Teleconsulta Regular]
    
    F --> I[Atualização Automática no Prontuário Vivo]
    G --> I
    H --> I
    
    I --> J[Nurse Blua: Acompanhamento contínuo de hábitos via WhatsApp]
