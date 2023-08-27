package com.ihub.www;

import java.io.IOException;
import java.io.PrintWriter;

import javax.servlet.RequestDispatcher;
import javax.servlet.ServletException;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

public class LoginSrv extends HttpServlet
{
	protected void doPost(HttpServletRequest req,HttpServletResponse res)throws ServletException,IOException
	{
		PrintWriter pw=res.getWriter();
		res.setContentType("text/html");
		
		String uname=req.getParameter("uname");
		String upwd=req.getParameter("upwd");
		
		RequestDispatcher rd=null;
		
		if(uname.equals("raja") && upwd.equals("rani"))
		{
			rd=req.getRequestDispatcher("success.html");
			rd.forward(req, res);
		}
		else
		{
			rd=req.getRequestDispatcher("failure.html");
			rd.forward(req, res);
		}
			
	}
}








