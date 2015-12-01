// Strings de tamanho ilimitado.

struct texto_inicio {

    struct texto_continuacao
            o_texto_propriamente_dito;
};

struct texto_continuacao {

    unsigned int
            comprimento_atual;

    unsigned int
            comprimento_maximo_do_segmento;

    char *
            o_segmento_de_texto;

    unsigned int
            fim_do_texto
         :  1;

    struct texto_continuacao
            proximo_segmento;
};
