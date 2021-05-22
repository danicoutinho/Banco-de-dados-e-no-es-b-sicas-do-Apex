# Banco-de-dados-e-no-es-b-sicas-do-Apex
Desafio: Create a method for inserting accounts
public class AccountHandler {

    public static Account insertNewAccount(String actName){
        Account act = new Account(Name=actName);
        try{
            insert act;
            return act;
        }catch(DMLException e){
            system.debug('DML Exception: ' + e);
            return null;
        }
    }
}
