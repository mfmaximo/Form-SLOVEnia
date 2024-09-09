# Form-SLOVEnia
Forms
# Saving the form content in HTML and making it available for download

html_content = """
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cadastro e Confirmação de Presença – Visita da Embaixadora da Eslovênia a Belo Horizonte</title>
    <link href='https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css' rel='stylesheet'>
</head>
<body style='background-color: #f5f5f5;'>
    <div class='container mt-5'>
        <div class='card'>
            <div class='card-header text-center' style='background-color: #006400; color: white;'>
                <h2>Cadastro e Confirmação de Presença – Visita da Embaixadora da Eslovênia a Belo Horizonte</h2>
            </div>
            <div class='card-body'>
                <p>Dragi prijatelji in prijateljice,</p>
                <p>(Queridos amigos e amigas),</p>
                <p>Estamos formando um cadastro da comunidade eslovena em Minas Gerais para manter todos informados sobre eventos, encontros e oportunidades ligadas à Eslovênia.
                Agradecemos por preencher este formulário para que possamos fortalecer os laços da nossa comunidade e planejar o jantar de confraternização.
                Najlepša hvala! (Muito obrigado!)</p>

                <form>
                    <div class='mb-3'>
                        <label for='nomeCompleto' class='form-label'>1. Nome Completo</label>
                        <input type='text' class='form-control' id='nomeCompleto' placeholder='Digite seu nome completo'>
                    </div>
                    <div class='mb-3'>
                        <label for='email' class='form-label'>2. E-mail</label>
                        <input type='email' class='form-control' id='email' placeholder='Digite seu e-mail'>
                    </div>
                    <div class='mb-3'>
                        <label for='telefone' class='form-label'>3. Telefone (WhatsApp ou outro)</label>
                        <input type='text' class='form-control' id='telefone' placeholder='Digite seu número de telefone'>
                    </div>
                    <div class='mb-3'>
                        <label for='vinculo' class='form-label'>4. Qual o seu vínculo com a Eslovênia?</label>
                        <select class='form-select' id='vinculo'>
                            <option>Sou descendente de eslovenos.</option>
                            <option>Sou casado(a) com alguém de origem eslovena.</option>
                            <option>Tenho interesse na cultura e no país.</option>
                            <option>Outro (especificar)</option>
                        </select>
                    </div>
                    <div class='mb-3'>
                        <label class='form-label'>5. Você irá participar do seminário no dia 24 de setembro (ACMinas, 16h00 às 18h00)?</label><br>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='seminario' id='seminarioSim' value='Sim'>
                            <label class='form-check-label' for='seminarioSim'>Sim</label>
                        </div>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='seminario' id='seminarioTalvez' value='Talvez'>
                            <label class='form-check-label' for='seminarioTalvez'>Ainda não tenho certeza</label>
                        </div>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='seminario' id='seminarioNao' value='Não'>
                            <label class='form-check-label' for='seminarioNao'>Não poderei comparecer</label>
                        </div>
                    </div>
                    <div class='mb-3'>
                        <label class='form-label'>6. Você irá participar do jantar de confraternização no Restaurante Neckartal (por adesão)?</label><br>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='jantar' id='jantarSim' value='Sim, com certeza!'>
                            <label class='form-check-label' for='jantarSim'>Sim, com certeza!</label>
                        </div>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='jantar' id='jantarTalvez' value='Ainda não tenho certeza'>
                            <label class='form-check-label' for='jantarTalvez'>Ainda não tenho certeza</label>
                        </div>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='jantar' id='jantarNao' value='Não poderei comparecer'>
                            <label class='form-check-label' for='jantarNao'>Não poderei comparecer</label>
                        </div>
                    </div>
                    <div class='mb-3'>
                        <label class='form-label'>7. Quantas pessoas irão com você ao jantar (incluindo você)?</label>
                        <select class='form-select' id='numPessoas'>
                            <option>1 (somente eu)</option>
                            <option>2 (eu e um acompanhante)</option>
                            <option>3</option>
                            <option>4</option>
                            <option>Outro (especificar)</option>
                        </select>
                    </div>
                    <div class='mb-3'>
                        <label for='acompanhantes' class='form-label'>8. Informe os nomes dos seus acompanhantes (opcional)</label>
                        <input type='text' class='form-control' id='acompanhantes' placeholder='Digite os nomes dos seus acompanhantes'>
                    </div>
                    <div class='mb-3'>
                        <label for='restricaoAlimentar' class='form-label'>9. Você ou algum acompanhante tem alguma restrição alimentar?</label>
                        <input type='text' class='form-control' id='restricaoAlimentar' placeholder='Informe restrições alimentares, se houver'>
                    </div>
                    <div class='mb-3'>
                        <label class='form-label'>10. Você tem interesse em agendar um atendimento consular durante a visita da Embaixadora?</label><br>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='atendimentoConsular' id='consularSim' value='Sim'>
                            <label class='form-check-label' for='consularSim'>Sim</label>
                        </div>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='atendimentoConsular' id='consularNao' value='Não'>
                            <label class='form-check-label' for='consularNao'>Não</label>
                        </div>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='atendimentoConsular' id='consularTalvez' value='Talvez no futuro'>
                            <label class='form-check-label' for='consularTalvez'>Talvez no futuro, gostaria de ser informado.</label>
                        </div>
                    </div>
                    <div class='mb-3'>
                        <label class='form-label'>11. Você gostaria de receber atualizações e convites para eventos futuros?</label><br>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='atualizacoes' id='atualizacoesEmail' value='E-mail'>
                            <label class='form-check-label' for='atualizacoesEmail'>Sim, por e-mail</label>
                        </div>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='atualizacoes' id='atualizacoesWhatsapp' value='WhatsApp'>
                            <label class='form-check-label' for='atualizacoesWhatsapp'>Sim, por WhatsApp</label>
                        </div>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='atualizacoes' id='atualizacoesAmbos' value='Ambos'>
                            <label class='form-check-label' for='atualizacoesAmbos'>Sim, por ambos</label>
                        </div>
                        <div class='form-check'>
                            <input class='form-check-input' type='radio' name='atualizacoes' id='atualizacoesNao' value='Não'>
                            <label class='form-check-label' for='atualizacoesNao'>Não, obrigado</label>
                        </div>
                    </div>
                    <div class='mb-3'>
                        <label for='sugestoes' class='form-label'>12. Tem sugestões de atividades ou temas para nossos próximos encontros?</label>
                        <textarea class='form-control' id='sugestoes' rows='3' placeholder='Escreva aqui suas sugestões'></textarea>
                    </div>
                    <button type='submit' class='btn btn-primary'>Enviar</button>
                </form>
                <div class='text-center mt-4'>
                    <p>Naj
