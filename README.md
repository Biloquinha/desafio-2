on bd_caso_estudo_vendas.*
to danielgomes@localhost;
/*Aplicativo permissao de inserçao em todas as tabelas do banco*/
grant insert
on bd_caso_estudo_vendas.*
to danielgomes@localhost;
/*Aplicando permissao de banco insercao em todas as tabela definida*/
grant insert
on bd_caso_estudo_vendas.tb_prod
to danielgomes@localhost;
grant insert, update, delete
on `bd_caso_estudo_vendas`.`tb_func`
to root@localhost;

revoke insert, update
on `bd_caso_estudo_vendas`.`tb_func`
from root@localhost;

grant delete
on `bd_caso_estudo_vendas`.`tb_func`
to root@localhost;

revoke select
on `bd_caso_estudo_vendas`.`tb_func`
from root@localhost;

grant insert 
on `bd_caso_estudo_vendas`.`tb_func`
to root@localhost;
