# <h1> Banco de Dados </h1>
<p> Esse trablalho é voltado para ajudar na organização de um curso, tendo como principais entidades<br> curso, turma e aluno, como solicitado, e além dessas, disciplina e professor.<p>
<h2>Curso</h2>
<p> 
<li> <b>cod_curso</b> = Chave primária, única, não pode ser reutilizado, auto-increment (INT)</li>
<li>nome = Nome do curso (VARCHAR)</li>
<li>tipo = Se é presencial ou Ensino a Distancia (VARCHAR) </li>
<li>carga_horaria = Tempo necessário para conclusão do curso (INT) </li>
</p>
<h2>Turma</h2>
<p>
<li> <b>cod_turma</b> = Chave primária (INT) </li>
<li>matricula = Número da matricula do aluno. Chave estrangeira (INT)</li>
<li>cod_disc = Onde contem a grade curricular utilizada nas aulas. Chave estrangeira (INT)</li>
<li>cod_curso = Código que representa qual curso a turma está fazendo. Chave estrangeira (INT)</li>
</p>
<h2>Aluno</h2>
<p>
<li> <b>matricula</b> = Chave primária, número de identificação (INT)</li>
<li>nome = Nome do aluno (VARCHAR) </li>
<li>endereço = Informação de onde reside este aluno (VARCHAR)</li>
<li>tel = Telefone para contato (INT)</li>
</p>
<h2>Disciplina</h2>
<p>
<li> <b>cod_disc</b> = Chave primária (INT)</li>
<li>matricula_prof = Especialidade do professor. Chave secundária (INT)</li>
<li>grad_curricular (VARCHAR)</li>
</p>
<h2>Professor</h2>
<p>
<li> <b>matricula_prof</b> = Chave primária, número de indentificação (INT)</li>
<li>nome = Nome do professor (VARCHAR)</li>
<li>especialidade = Em qual área leciona (VARCHAR)</li>
<li>data_admição = Data em que foi contratado (DATE)</li>
</p>
<br>
<h1>Como essas essas estidades estão relacionadas?</h1>
<p>O curso esta relacionado com as turmas, pos está abrindo novas classes, e também está relacionado ao professor pois a implementação de novas classes almenta a demanda de contratações, a disciplina está relacionada com as turmas, e também com o professor para que  cada professor seja alocado nas turmas de acordo com a sua especialidade, e as turmas estão relacionadas com o aluno.
