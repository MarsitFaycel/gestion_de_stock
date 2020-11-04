
## Projet de gestion de stock avec spring MVC

# 1-configuration de projet

	1-presistence.xml
	
	2-applicationContext.xml 
	
	3-pom.xml (dependecies)


# 2-Generation des entites
	
	1- Article
	
	2- Category
	
	3- Client
	
	4- CommandeClient
	
	5- CommandeFournisseur
	
	6-Fournisseur
	
	7-ligneCommandeClient
	
	8-ligneCommandeFournisseur
	
	9- ligne Vente
	
	10- MVTSTK
	
	11- Utilisateur
	
	12- Vente
	
	13- relation onetomany
	
# 3-couche DAO
	
	1-creation interface dao generique IGenericDao
			
			public E save(E entity);
	
			public E update(E entity);
	
			public List<E> selectAll();
	
			public E getById(Long id);
			
			public void remove(Long id);
			
			public List<E> selectAll(String sortField, String sort);
			
			public E findOne(String paramName,Object paramValue);
			
			public E findOne(String[] paramNames, Object[]paramValues);
			
			public int findCountBy(String paramName ,String paramValue);

	2-classe GenericDaoImpl